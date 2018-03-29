# Ubuntu - just source this file

(grep '^precedence' /etc/gai.conf >>/dev/null || echo precedence ::ffff:0:0/96 100 >> /etc/gai.conf) &&
apt-get update &&
apt-get install git-core &&
git clone https://github.com/clockwork-nixie/setup-linode ~/.clockwork &&
. ~/.clockwork/setup

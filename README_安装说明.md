# Debug网页修复补丁

## 一键修复命令
```bash
cd /etc/formlabs/alternatives/current/lib/formlabs/apps/diesel/debug_web_ui && \
wget -q -O - https://raw.githubusercontent.com/Lucky-0105-tech/debug-web-ui-fix/main/debug_web_ui_fix.patch | git apply && \
pip3 install eventlet && \
/etc/init.d/debug-web-ui restart

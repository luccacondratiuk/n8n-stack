FROM n8nio/runners:1.121.0
USER root
RUN cd /opt/runners/task-runner-javascript && pnpm add moment uuid libphonenumber-js lodash crypto bcryptjs
RUN cd /opt/runners/task-runner-python && uv pip install numpy pandas cryptography
COPY n8n-task-runners.json /etc/n8n-task-runners.json
USER runner

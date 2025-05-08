FROM node:24.0-bullseye-slim@sha256:0139f0a20522ccf10ac39ed57dab5a108e996f11c1dff240cc334086bbe01f0e as node-base


FROM node-base as node-http-auth
ARG NODE_APP=.
ARG NODE_APP_NAME=http-service/server
# Add an env to save ARG
ENV NODE_APP_PATH "/app/${NODE_APP_NAME}"
COPY "$NODE_APP" /app
# Dont use exec form to interpolate correctly
CMD node $NODE_APP_PATH

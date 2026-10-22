FROM node:22.23.4-bookworm-slim

WORKDIR /app
ENV NODE_ENV=production

COPY --chown=node:node package.json ./
COPY --chown=node:node src ./src

USER node
EXPOSE 5173
CMD ["node", "src/server.js"]

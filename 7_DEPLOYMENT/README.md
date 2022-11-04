# Deployment

## Introduction

There are 2 ways for deploying:
1 - push (to server)
2 - pull (from server)

## Push method

- `scp` (sftp)
- `rsync`

eg.

```bash
scp -r build/. jimmylefevre@34.27.197.4:/home/jimmylefevre/front
```

-or-

```bash
rsync -avz build/. jimmylefevre@34.27.197.4:/home/jimmylefevre/front
```

TODO:

### Storage & Persistence
- [ ] Migrate `hostPath` to `persistentVolumeClaim` (standardize storage)
- [ ] Check backup/restore flow for PVC

### Image, Resources & Security
- [ ] Fork upstream repo -> build/push to private `ghcr.io`
- [ ] Update manifests to pull image from `ghcr.io`

### Access from internet
- [ ] Configure cloudflared (change current tunnel from docker-compose based app to k3s one)
- [ ] Stop docker-compose based app to finish migration


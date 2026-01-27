TODO:

### Storage & Persistence
- [ ] Migrate `nodePath` to `persistentVolumeClaim` (standardize storage)
- [ ] Check backup/restore flow for PVC

### CI/CD Pipeline (GitHub Actions)
- [ ] **Linting & Validation:**
    - [x] Add `yamllint` for manifest consistency
    - [x] Add `kubeconform` for schema validation
    - [ ] Test with `kubectl --dry-run`
- [ ] **Security:**
    - [ ] `trivy` for image/config scanning
    - [ ] `gitleaks` to prevent secret commits
- [ ] **Automation UX:**
    - [ ] Setup `path filtering` (only run jobs when relevant files change)
    - [ ] Generate `PR summary` for better visibility

### Image, Resources & Security
- [ ] Fork upstream repo -> build/push to private `ghcr.io`
- [ ] Update manifests to pull image from `ghcr.io`
- [x] Add `resources` (limits/requests) to deployment
- [x] Add `securityContext` (rootless, capabilities, etc.)

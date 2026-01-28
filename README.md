# infra-k3s

TODO:

### CI/CD Pipeline (GitHub Actions)
- [x] **Linting & Validation:**
    - [x] Add `yamllint` for manifest consistency
    - [x] Add `kubeconform` for schema validation
- [x] **Security:**
    - [x] `trivy` for image/config scanning
    - [x] `gitleaks` to prevent secret commits
- [ ] **Automation UX:**
    - [ ] Setup `path filtering` (only run jobs when relevant files change)
    - [ ] Generate `PR summary` for better visibility
- [ ] **Other:**
    - [ ] Make sure that current gha run is stopped if new commit was pushed - avoid concurency

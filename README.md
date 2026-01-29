# infra-k3s

TODO:

### CI/CD Pipeline (GitHub Actions)
- [x] **Linting & Validation:**
    - [x] Add `yamllint` for manifest consistency
    - [x] Add `kubeconform` for schema validation
- [x] **Security:**
    - [x] `trivy` for image/config scanning
    - [x] `gitleaks` to prevent secret commits
    - [ ] another trivy scan for medium and low - not failing pipeline, but showing issues
- [x] **Other:**
    - [x] Make sure that current gha run is stopped if new commit was pushed - avoid concurency

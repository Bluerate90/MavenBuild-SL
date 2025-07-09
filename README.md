# DevOps Portfolio: Java CI/CD Pipeline Demo

## Project Overview
This project demonstrates a complete CI/CD pipeline using GitHub Actions, Maven, and Jenkins for a Java web application.

## 🚀 Technologies Used
- **Version Control**: Git, GitHub
- **Build Tool**: Maven
- **CI/CD**: GitHub Actions, Jenkins
- **Languages**: Java, YAML, Shell Scripting
- **Deployment**: Tomcat Server
- **Infrastructure**: Linux (Ubuntu)

## 🔧 Pipeline Architecture

### 1. **GitHub Actions (CI)**
- **Trigger**: On every push to main branch
- **Steps**:
  - Checkout code
  - Setup Java 11 and Maven
  - Run unit tests
  - Build WAR file
  - Upload artifacts
  - Trigger Jenkins deployment

### 2. **Jenkins (CD)**
- **Trigger**: Remote API call from GitHub Actions
- **Steps**:
  - Pull artifacts from GitHub
  - Deploy to Tomcat server
  - Run health checks
  - Send notifications

## 🚀 Key Features Demonstrated

### DevOps Practices
- ✅ **Continuous Integration**: Automated testing and building
- ✅ **Continuous Deployment**: Automated deployment to staging
- ✅ **Infrastructure as Code**: Pipeline configuration in YAML
- ✅ **Automated Testing**: Unit tests integrated in pipeline
- ✅ **Artifact Management**: Secure artifact storage and transfer
- ✅ **Remote Deployment**: SSH-based deployment to remote servers

### Technical Skills
- ✅ **GitHub Actions**: Workflow creation and management
- ✅ **Jenkins**: Job configuration and API integration
- ✅ **Maven**: Build automation and dependency management
- ✅ **Linux Administration**: Server management and scripting
- ✅ **Shell Scripting**: Automation scripts
- ✅ **Java Development**: Web application development
- ✅ **Tomcat**: Application server deployment

## 📊 Pipeline Metrics
- **Build Time**: ~3-5 minutes
- **Test Coverage**: Unit tests included
- **Deployment Time**: ~2-3 minutes
- **Success Rate**: 95%+ (with proper configuration)

## 🔒 Security Features
- **Credential Management**: Secure storage of passwords and tokens
- **SSH Key Authentication**: Secure remote server access
- **Token-based Authentication**: Jenkins API security
- **Artifact Integrity**: Checksum verification

## 📈 Monitoring & Observability
- **Build Status**: Real-time build status in GitHub
- **Deployment Logs**: Detailed logging for troubleshooting
- **Health Checks**: Automated application health verification
- **Notifications**: Slack/Email integration for build status

## 🔧 Getting Started

### Prerequisites
- Java 11 or higher
- Maven 3.6+
- Jenkins server
- Tomcat server
- GitHub account with Actions enabled

### Setup Instructions
1. **Fork this repository**
2. **Configure GitHub Secrets**:
   - `JENKINS_HOST`: Your Jenkins server IP
   - `JENKINS_USER`: Jenkins username
   - `JENKINS_PASS`: Jenkins password
   - `DEPLOY_USER`: Deployment server username
   - `DEPLOY_PASS`: Deployment server password

3. **Configure Jenkins Job**:
   - Create new job named "build-job"
   - Enable remote API trigger
   - Set authentication token

4. **Deploy**:
   - Push code to trigger pipeline
   - Monitor build in Actions tab
   - Verify deployment on target server

## 🐛 Troubleshooting

### Common Issues
- **Jenkins job not triggering**: Check authentication and job name
- **Build failures**: Verify Java/Maven versions
- **Deployment failures**: Check server connectivity and permissions

### Debugging Steps
1. Check GitHub Actions logs
2. Verify Jenkins server status
3. Test SSH connectivity
4. Validate Maven configuration

## 🎯 Future Enhancements
- [ ] Docker containerization
- [ ] Kubernetes deployment
- [ ] SonarQube integration
- [ ] Performance testing
- [ ] Blue-green deployment
- [ ] Infrastructure monitoring

## 👨‍💻 Author
**[Tibyan Hussien]** - DevOps Engineer

## 📄 License
This project is licensed under the MIT License.

---

*This project demonstrates real-world DevOps practices and can be used as a reference for CI/CD pipeline implementation.*

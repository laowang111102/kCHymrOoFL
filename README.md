## 前言

本项目是基于JavaWeb技术开发的城乡居民基本医疗信息管理系统。该系统旨在提高医疗信息管理的效率和安全性，为城乡居民提供更优质、更便捷的医疗服务。通过本系统，用户可以轻松管理病例、病人、药品、医生等各类医疗信息，确保数据的及时性和准确性。

## 内容介绍

本系统主要包括病例管理、病人管理、药品管理、医生管理、用户管理、管理员管理等功能模块。病例管理模块允许用户添加、修改、删除和查询病例信息；病人管理模块负责维护病人信息，包括个人基本信息、病历等；药品管理模块包括药品入库和使用管理，确保药品信息准确无误；医生管理模块涵盖医生信息维护、咨询和挂号管理；用户管理模块允许用户管理个人信息，如修改密码、更新联系方式等；管理员管理模块则提供系统管理功能，如用户权限管理、公告发布等。通过这些模块的紧密协作，本系统能够全面地记录和处理城乡居民的医疗信息，确保数据的及时性和准确性。

## 技术介绍

- **语言**：Java
- **使用框架**：Spring Boot
- **前端技术**：JS、Vue、css3
- **开发工具**：IDEA/Eclipse
- **数据库**：MySQL 5.7/8.0
- **数据库管理工具**：phpstudy/Navicat
- **JDK版本**：jdk1.8
- **Maven**：apache-maven 3.8.1-bin
- **前端环境**：Node.js 12/14/16

## 核心代码

```java
@Service
public class PatientService {

    @Autowired
    private PatientRepository patientRepository;

    public List<Patient> findAll() {
        return patientRepository.findAll();
    }

    public Patient findById(Long id) {
        return patientRepository.findById(id).orElse(null);
    }

    public Patient save(Patient patient) {
        return patientRepository.save(patient);
    }

    public void deleteById(Long id) {
        patientRepository.deleteById(id);
    }

    public Patient update(Long id, Patient patientDetails) {
        Patient patient = patientRepository.findById(id).orElseThrow(() -> new ResourceNotFoundException("Patient", "id", id));

        patient.setName(patientDetails.getName());
        patient.setAge(patientDetails.getAge());
        patient.setGender(patientDetails.getGender());
        patient.setPhoneNumber(patientDetails.getPhoneNumber());
        patient.setAddress(patientDetails.getAddress());

        return patientRepository.save(patient);
    }
}
```

## 免费源码获取

```
8000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img10.360buyimg.com/ddimg/jfs/t1/327704/39/4647/164038/689ea8dbFfe2f311a/6c0f2f2c2f69248b.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/320682/16/24741/107286/689ea8b9F2ddb4773/17ed4ba2fb119583.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/308832/29/26606/39894/689ea8b9Fe87e74b3/5df41f189d9fd73b.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/303364/24/27166/38629/689ea8baF83f95403/4fcfb8e83b21c312.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/310225/2/26575/28952/689ea8baF0e967304/fecb584dc418e5a0.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/315028/31/26552/19669/689ea8bbFdea45567/a7640afb13f8051f.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/319448/29/25325/95268/689ea8bcFb8dca683/5ba8c62623db57e6.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/311572/8/26394/44195/689ea8bcF25863e08/b9702159f2637af1.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/314236/13/26576/81713/689ea8beFbf9be6ab/ed4ebd2faba2d0ca.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/307838/2/26686/56588/689ea8beF2e0e7cf8/bddd060bbc60bd2e.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)

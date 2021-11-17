---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2cc3a781295db09bd09fdfc895588a8befadfc35035b012ee13ef30e72b861cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156952"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UrlAssessmentRequest threatAssessmentRequest = new UrlAssessmentRequest();
threatAssessmentRequest.url = "http://test.com";
threatAssessmentRequest.expectedAssessment = ThreatExpectedAssessment.BLOCK;
threatAssessmentRequest.category = ThreatCategory.PHISHING;

graphClient.informationProtection().threatAssessmentRequests()
    .buildRequest()
    .post(threatAssessmentRequest);

```
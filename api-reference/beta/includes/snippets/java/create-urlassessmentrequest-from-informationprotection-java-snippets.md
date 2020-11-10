---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e09393f6c225776e30989b58d9b42f37d4fc7981
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952960"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UrlAssessmentRequest threatAssessmentRequest = new UrlAssessmentRequest();
threatAssessmentRequest.url = "http://test.com";
threatAssessmentRequest.expectedAssessment = ThreatExpectedAssessment.BLOCK;
threatAssessmentRequest.category = ThreatCategory.PHISHING;

graphClient.informationProtection().threatAssessmentRequests()
    .buildRequest()
    .post(threatAssessmentRequest);

```
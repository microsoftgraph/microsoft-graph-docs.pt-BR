---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe4eef059b5f0b238b2512d741398747b6bc6896
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881536"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/users/14011"));

graphClient.education().classes("{class-id}").teachers().references()
    .buildRequest()
    .post(educationUser);

```
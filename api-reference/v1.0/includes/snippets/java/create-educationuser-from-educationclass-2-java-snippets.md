---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe4eef059b5f0b238b2512d741398747b6bc6896
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963720"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/users/14011"));

graphClient.education().classes("{class-id}").teachers().references()
    .buildRequest()
    .post(educationUser);

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4b6642b7eaeede7fd50e4605e38945f3227bb8ec
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136277"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategory educationCategory = new EducationCategory();
educationCategory.displayName = "Quizzes";

graphClient.education().classes("60eaa744-aa87-4276-b985-1633683119f8").assignmentCategories()
    .buildRequest()
    .post(educationCategory);

```
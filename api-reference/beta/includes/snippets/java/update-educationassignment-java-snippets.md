---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bac6831330abd39e0c21c97ce6ce648abea24e65
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860743"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignment educationAssignment = new EducationAssignment();
educationAssignment.displayName = "Week 1 reading assignment";
EducationItemBody instructions = new EducationItemBody();
instructions.contentType = BodyType.TEXT;
instructions.content = "Read chapters 1 through 3";
educationAssignment.instructions = instructions;
educationAssignment.dueDateTime = "2014-02-01T00:00:00Z";

graphClient.education().classes("11021").assignments("19002")
    .buildRequest()
    .patch(educationAssignment);

```
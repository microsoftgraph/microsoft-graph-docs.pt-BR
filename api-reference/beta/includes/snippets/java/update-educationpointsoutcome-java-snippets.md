---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b32da9f6aaa08f63b962338df346aa3589756393
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52254359"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationPointsOutcome educationOutcome = new EducationPointsOutcome();
EducationAssignmentPointsGrade points = new EducationAssignmentPointsGrade();
points.points = 85.0;
educationOutcome.points = points1;

graphClient.education().classes("{id}").assignments("{id}").submissions("{id}").outcomes("{id}")
    .buildRequest()
    .patch(educationOutcome);

```
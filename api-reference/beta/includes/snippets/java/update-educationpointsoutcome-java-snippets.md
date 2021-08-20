---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7b77d3c24c824739e7cbd1a2638db581e593376207c71b35a49b8f3bf8302653
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159418"
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
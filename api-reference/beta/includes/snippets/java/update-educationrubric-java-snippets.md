---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0c6160b4e2a4342b5331b25c7c70321d1f8f138e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965970"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubric educationRubric = new EducationRubric();
educationRubric.displayName = "Example Credit Rubric after display name patch";

graphClient.education().me().rubrics("{id}")
    .buildRequest()
    .patch(educationRubric);

```
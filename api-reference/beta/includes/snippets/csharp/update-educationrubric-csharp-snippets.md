---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6447352366b875c742fba85146016f723e0ad861420105b459b18b60e7b44ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217204"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRubric = new EducationRubric
{
    DisplayName = "Example Credit Rubric after display name patch"
};

await graphClient.Education.Me.Rubrics["{educationRubric-id}"]
    .Request()
    .UpdateAsync(educationRubric);

```
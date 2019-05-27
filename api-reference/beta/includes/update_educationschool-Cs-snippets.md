---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef7b372b4785b626b41c4ce11757c47426344eba
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468743"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = new EducationSchool
{
    DisplayName = "Fabrikam Arts High School",
    Description = "Magnate school for the arts. Los Angeles School District"
};

await graphClient.Education.Schools["10002"]
    .Request()
    .UpdateAsync(educationSchool);

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef7b372b4785b626b41c4ce11757c47426344eba
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714484"
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
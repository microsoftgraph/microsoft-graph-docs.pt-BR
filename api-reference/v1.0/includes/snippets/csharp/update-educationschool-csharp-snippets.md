---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba842a052edfb19e5f7333912aa979a91a704003
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732762"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = new EducationSchool
{
    DisplayName = "Fabrikam Arts High School",
    Description = "Magnate school for the arts. Los Angeles School District"
};

await graphClient.Education.Schools["{school-id}"]
    .Request()
    .UpdateAsync(educationSchool);

```
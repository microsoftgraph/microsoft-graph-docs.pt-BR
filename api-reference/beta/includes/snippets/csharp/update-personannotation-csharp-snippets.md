---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44cda98dd97e4b958981dbc4e1d95cf91feac416
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774177"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnnotation = new PersonAnnotation
{
    AllowedAudiences = AllowedAudiences.Organization
};

await graphClient.Users["{user-id}"].Profile.Notes["{personAnnotation-id}"]
    .Request()
    .UpdateAsync(personAnnotation);

```
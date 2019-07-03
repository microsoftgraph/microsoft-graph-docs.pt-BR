---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 710abecde2fe9a3c2fa60c2615c92853a31ccac3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463260"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.App.Calls["{id}"].AudioRoutingGroups["{id}"]
    .Request()
    .DeleteAsync();

```
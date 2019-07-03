---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8cddd844439f86ba66ecf43c9ec10f2e3a6ebe05
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465567"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var versions = await graphClient.Me.Drive.Items["{item-id}"].Versions["{version-id}"]
    .Request()
    .Select( e => new {
             e.Content 
             })
    .GetAsync();

var content = versions.Content;

```
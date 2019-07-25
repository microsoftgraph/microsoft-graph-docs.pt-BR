---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec75c089c31449e3d9bea579f26b95594120dd7b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733135"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "embed";

await graphClient.Me.Drive.Items["{item-id}"]
    .CreateLink(type,scope)
    .Request()
    .PostAsync();

```
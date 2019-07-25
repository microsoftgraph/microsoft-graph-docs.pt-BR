---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f04a543d91344345401916d600f10acea89bfed5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730507"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Root.Items.{item-id}.Permissions.{perm-id}
    .Request()
    .DeleteAsync();

```
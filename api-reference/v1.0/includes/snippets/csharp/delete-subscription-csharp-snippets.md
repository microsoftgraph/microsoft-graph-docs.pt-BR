---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4794d8788d3d40150f96f03065ef5f486232c699
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715694"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Subscriptions["{id}"]
    .Request()
    .DeleteAsync();

```
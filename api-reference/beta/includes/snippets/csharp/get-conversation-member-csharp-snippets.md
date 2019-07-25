---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0023d2a430b9edda902b8e22ad49161b82cc528
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707219"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Me.Chats["{id}"].Members
    .Request()
    .GetAsync();

```
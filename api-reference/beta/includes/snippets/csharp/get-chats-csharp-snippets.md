---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5abc9ccd9e4790bcaa7b5dda3fdadc3d114ac0a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707730"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chats = await graphClient.Users["{id}"].Chats
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39b1c2db4bcf38c17f178e71a8ee0489e1d59a6b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707772"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = await graphClient.Users["{id}"].Chats["{id}"]
    .Request()
    .GetAsync();

```
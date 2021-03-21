---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24450709498dbd470d75ddd2ab4c93656c0de222
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957097"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Users["{user-id}"].Manager
    .Request()
    .GetAsync();

```
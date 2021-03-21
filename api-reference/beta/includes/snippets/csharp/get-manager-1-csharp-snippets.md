---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 476deaf2230c254e3fd5e78cc2b98a2c8156db2b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957766"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Contacts["{orgContact-id}"].Manager
    .Request()
    .GetAsync();

```
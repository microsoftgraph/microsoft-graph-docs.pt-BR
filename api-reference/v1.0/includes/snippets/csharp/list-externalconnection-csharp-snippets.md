---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1151894523cbf9169a00f0618cf36b3859eb17cd
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696817"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connections = await graphClient.External.Connections
    .Request()
    .GetAsync();

```
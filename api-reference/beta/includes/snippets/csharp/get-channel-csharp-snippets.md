---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8962445fc41eb169eff91bd17c6c88e7e693682
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708667"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = await graphClient.Teams["{id}"].Channels["{id}"]
    .Request()
    .GetAsync();

```
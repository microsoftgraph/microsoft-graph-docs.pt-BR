---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51698e78003b188cfabf399d4f93d32ffd28d9cb
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565622"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printOperation = await graphClient.Print.Operations["{id}"]
    .Request()
    .GetAsync();

```
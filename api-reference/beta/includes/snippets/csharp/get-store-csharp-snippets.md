---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03706001a0fa80548c08b2ec7fecc5c1b81f5830
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565807"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var store = await graphClient.TermStore
    .Request()
    .GetAsync();

```
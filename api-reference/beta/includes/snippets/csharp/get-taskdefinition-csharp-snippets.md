---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca6fee6b311f5742da4a429835799ab63510d6f0
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565305"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTaskDefinition = await graphClient.Print.TaskDefinitions["fab143fd-ee61-4358-8558-2c7dee953982"]
    .Request()
    .GetAsync();

```
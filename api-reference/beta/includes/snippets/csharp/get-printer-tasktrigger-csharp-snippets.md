---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21ccea189c21cca468a33a69f1ccfff4135deea3
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTaskTrigger = await graphClient.Print.Printers["{printerId}"].TaskTriggers["{taskTriggerId}"]
    .Request()
    .GetAsync();

```
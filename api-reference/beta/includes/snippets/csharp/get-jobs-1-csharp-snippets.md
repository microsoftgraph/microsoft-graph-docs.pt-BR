---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 934d086467b072d6d2c8d682eff177053f322c06
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960909"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var jobs = await graphClient.Print.Printers["{printer-id}"].Jobs
    .Request()
    .GetAsync();

```
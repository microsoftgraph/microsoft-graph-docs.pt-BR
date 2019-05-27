---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4d99ea02357dd00035d49eef2cccbe3767ede4e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463017"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Messages["AAMkADA1M-zAAA="].Attachments["AAMkADA1M-CJKtzmnlcqVgqI="]
    .Request()
    .GetAsync();

```
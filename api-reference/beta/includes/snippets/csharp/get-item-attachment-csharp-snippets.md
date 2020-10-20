---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4d99ea02357dd00035d49eef2cccbe3767ede4e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622105"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Messages["AAMkADA1M-zAAA="].Attachments["AAMkADA1M-CJKtzmnlcqVgqI="]
    .Request()
    .GetAsync();

```
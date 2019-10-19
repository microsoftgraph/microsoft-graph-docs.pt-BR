---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4d99ea02357dd00035d49eef2cccbe3767ede4e
ms.sourcegitcommit: 6deec57c0ab736260ee3599703bfd3f567ee6d82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2019
ms.locfileid: "35739180"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Messages["AAMkADA1M-zAAA="].Attachments["AAMkADA1M-CJKtzmnlcqVgqI="]
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 795a14729d85d3262edc6e7aa6a5be05aad21b4a
ms.sourcegitcommit: 6deec57c0ab736260ee3599703bfd3f567ee6d82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2019
ms.locfileid: "35739181"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Messages["AAMkADA1M-zAAA="].Attachments["AAMkADA1M-CJKtzmnlcqVgqI="]
    .Request()
    .Expand("itemattachment/item")
    .GetAsync();

```
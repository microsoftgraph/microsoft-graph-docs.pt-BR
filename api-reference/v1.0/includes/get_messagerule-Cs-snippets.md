---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6cdcf72e45bb8eb3d2dd5361fbc8a349682a6a8c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461069"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageRule = await graphClient.Me.MailFolders["inbox"].MessageRules["AQAAAJ5dZqA="]
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5587acf5f6bf337baf1a6011089c4511fa5c385
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458821"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.MailFolders["{id}"]
    .Request()
    .DeleteAsync();

```
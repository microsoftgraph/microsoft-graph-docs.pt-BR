---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6bd4665a76282fe1e553b2f9e1255d0358b0eef
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460942"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "embed";

await graphClient.Me.Drive.Items["{item-id}"]
    .CreateLink(type,scope,expirationDateTime,password,message,recipients)
    .Request()
    .PostAsync();

```
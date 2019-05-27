---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0948b00d09234f10da6195edbe21d7b64d9a36ee
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childFolders = await graphClient.Me.MailFolders["searchfolders"].ChildFolders
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f34e97d12099d0cd49a53787b6877f507790f8e3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444073"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.MailFolders["{id}"].Messages.Delta()
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 42d8cc8ece6e8724773ace6284a27edb933348a5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472711"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childFolders = await graphClient.Me.MailFolders["AAMkAGVmMDEzM"].ChildFolders
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 370632d663378d6cb195f2b8de50b5c628e193ecb2760fa336fc7e338f5bde75
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406910"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].FilesFolder
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43406fcf1c6a039213a54d2d8149ff553de411ed4633282cb0ecf77a90050f08
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158982"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Sites["{site-id}"].Drives
    .Request()
    .GetAsync();

```
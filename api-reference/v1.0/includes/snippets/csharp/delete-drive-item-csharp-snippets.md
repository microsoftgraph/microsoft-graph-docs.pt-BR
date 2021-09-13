---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a453660cb77a20a763b20bbf35b7454b824f010745f2aa458b57a64745f843ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272784"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Request()
    .DeleteAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 884dc370b05c3eedbca5c58cfb1f1873f67ebb7a7f2b6e953c72160c6c747a8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159268"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "embed";

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .CreateLink(type,null,null,null,null)
    .Request()
    .PostAsync();

```
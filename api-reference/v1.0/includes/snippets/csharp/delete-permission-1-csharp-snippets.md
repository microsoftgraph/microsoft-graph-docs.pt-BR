---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a2d41a7c1b96a19580fcfb382d82eac8b127afae
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945095"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Permissions["{permission-id}"]
    .Request()
    .DeleteAsync();

```
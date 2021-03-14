---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d85951efc0cba3c93a91e345086e6e2acaf5ea16
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Users["{user-id}"].Drives
    .Request()
    .GetAsync();

```
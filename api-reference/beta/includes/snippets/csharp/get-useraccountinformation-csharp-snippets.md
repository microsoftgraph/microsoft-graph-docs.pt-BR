---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66eedb437dc6d93b9cd2201950d280f0a89791a0e0ba8827f6152c1b9dfb6f1a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217607"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAccountInformation = await graphClient.Me.Profile.Account["{userAccountInformation-id}"]
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93aae139444e5dfa824999a1e569834dc47d7a93efb36ef82529a6df09e1d198
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327939"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var followedSites = await graphClient.Me.FollowedSites
    .Request()
    .GetAsync();

```
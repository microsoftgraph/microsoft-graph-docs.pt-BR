---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1b3b8803ce6424a77533679ec6722663e3d4cdb723bd1423293429057fa214d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102275"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personInterest = await graphClient.Me.Profile.Interests["{personInterest-id}"]
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c91030fc25ed95f41c96aadaf2be586387ad23a7401250c56b4300003e75f32f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156526"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{application-id}"].TokenLifetimePolicies["{tokenLifetimePolicy-id}"].Reference
    .Request()
    .DeleteAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf426dd0368e845e0b81e1880bc3b11893cda3d00d0ae0f78fc2c18849dccff6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159696"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocations = await graphClient.Identity.ConditionalAccess.NamedLocations
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7a5e30f02e355e129e17806da317987f18d4679f
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994139"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackages = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages
    .Request()
    .GetAsync();

```
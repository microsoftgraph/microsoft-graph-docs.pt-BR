---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96749efe0513838b967cd4008f6d86ba6b67e3bd
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994239"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageCatalogs = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs
    .Request()
    .GetAsync();

```
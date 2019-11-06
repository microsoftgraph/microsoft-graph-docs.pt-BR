---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56bd753698e1d421a0dc36a5e32852f7f7ac5ebe
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994267"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResources = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["{id}"].AccessPackageResources
    .Request()
    .GetAsync();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7179b7b0c22d84511377fd56c7a726238b7eedffb1c83675cefd8c1eaf150009
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099846"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageCatalog = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["{accessPackageCatalog-id}"]
    .Request()
    .GetAsync();

```
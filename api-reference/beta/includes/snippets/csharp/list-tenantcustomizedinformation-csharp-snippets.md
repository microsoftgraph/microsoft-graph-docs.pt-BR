---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82489dd3a37ef2be30ea6f862a64a1258e358997
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440623"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantsCustomizedInformation = await graphClient.TenantRelationships.ManagedTenants.TenantsCustomizedInformation
    .Request()
    .GetAsync();

```
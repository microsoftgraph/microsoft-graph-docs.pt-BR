---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6a221c90b78cb00a2ded9c63c630597392601ba
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441391"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUser = await graphClient.TenantRelationships.ManagedTenants.RiskyUsers["{managedTenants.riskyUser-id}"]
    .Request()
    .GetAsync();

```
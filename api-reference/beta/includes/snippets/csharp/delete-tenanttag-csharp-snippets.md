---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c509eeb78998df390ed959f332c6944bf14fd8dd
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441116"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TenantRelationships.ManagedTenants.TenantTags["{managedTenants.tenantTag-id}"]
    .Request()
    .DeleteAsync();

```
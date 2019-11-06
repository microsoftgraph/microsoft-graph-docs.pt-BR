---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 304074d9f8394e792de106189acc0b305e98a5b6
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994349"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageCatalog = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["{id}"]
    .Request()
    .GetAsync();

```
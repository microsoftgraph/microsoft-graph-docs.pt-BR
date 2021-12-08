---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4390f42382fc4fa016bb14394fe974af6368726
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61335632"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageCatalog = await graphClient.IdentityGovernance.EntitlementManagement.Catalogs["{accessPackageCatalog-id}"]
    .Request()
    .GetAsync();

```
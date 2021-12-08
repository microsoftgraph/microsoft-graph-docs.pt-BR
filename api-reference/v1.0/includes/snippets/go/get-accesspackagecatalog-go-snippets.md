---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4028629ae9430207ad16d3ac9368ef74d48f87c9
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61335619"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageCatalogId := "accessPackageCatalog-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().CatalogsById(&accessPackageCatalogId).Get(nil)


```
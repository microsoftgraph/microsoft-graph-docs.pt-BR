---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9abb8916738ed53edf3f9ed04ee118384492308e
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347001"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageCatalogId := "accessPackageCatalog-id"
graphClient.IdentityGovernance().EntitlementManagement().CatalogsById(&accessPackageCatalogId).Delete(nil)


```
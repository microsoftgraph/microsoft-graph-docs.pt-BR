---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72bc2d0d8b53a78642a4c9b4260d39bae128c090
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322625"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageCatalog()
displayName := "Catalog One"
requestBody.SetDisplayName(&displayName)
accessPackageCatalogId := "accessPackageCatalog-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogsById(&accessPackageCatalogId).Patch(requestBody)


```
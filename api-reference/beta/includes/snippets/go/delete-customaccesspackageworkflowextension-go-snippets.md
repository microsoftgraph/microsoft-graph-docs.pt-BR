---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8fd569852d872088bbad33536817dbd0883bdf90
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410770"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageCatalogId := "accessPackageCatalog-id"
customAccessPackageWorkflowExtensionId := "customAccessPackageWorkflowExtension-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogsById(&accessPackageCatalogId).CustomAccessPackageWorkflowExtensionsById(&customAccessPackageWorkflowExtensionId).Delete(nil)


```
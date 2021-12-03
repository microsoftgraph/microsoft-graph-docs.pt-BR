---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b75434e329ff299c6953ed9f2a2c09a9a1e0bb74
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285843"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageId := "accessPackage-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackagesById(&accessPackageId).Delete(nil)


```
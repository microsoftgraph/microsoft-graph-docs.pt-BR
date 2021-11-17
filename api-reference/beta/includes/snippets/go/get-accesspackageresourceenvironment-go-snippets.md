---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e517a754d7453253eeee9b1c9b23540863c6687f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988214"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessPackageResourceEnvironmentId := "accessPackageResourceEnvironment-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceEnvironmentsById(&accessPackageResourceEnvironmentId).Get(options)


```
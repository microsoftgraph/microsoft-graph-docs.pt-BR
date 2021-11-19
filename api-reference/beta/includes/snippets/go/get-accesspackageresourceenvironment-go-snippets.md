---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81697fe614f45c0694e863d55fc0bd3272e92051
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087555"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageResourceEnvironmentId := "accessPackageResourceEnvironment-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceEnvironmentsById(&accessPackageResourceEnvironmentId).Get(options)


```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 145dcacfaf92d47c6c90f95dac959d90e48da3f0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314297"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters{
    Filter: "isElevated%20eq%20true",
}
options := &msgraphsdk.PrivilegedRoleAssignmentsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.PrivilegedRoleAssignments().GetWithRequestConfigurationAndResponseHandler(options, nil)


```
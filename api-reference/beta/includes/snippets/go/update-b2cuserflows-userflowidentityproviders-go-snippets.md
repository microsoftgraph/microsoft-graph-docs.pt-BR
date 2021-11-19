---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee3c97713fa8ddaa9d5cb48734414c29ff530958
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093706"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/identity/identityProviders/{id}",
    "@odata.type": "#microsoft.graph.identityProvider",
}
options := &msgraphsdk.RefRequestBuilderPatchOptions{
    Body: requestBody,
}
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).UserFlowIdentityProviders().$ref().Patch(options)


```
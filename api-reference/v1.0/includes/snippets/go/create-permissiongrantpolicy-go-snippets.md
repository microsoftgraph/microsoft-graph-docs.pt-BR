---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6e7613bbd14c4a38b52a5bd2e26c4d83653441f3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324614"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPermissionGrantPolicy()
id := "my-custom-consent-policy"
requestBody.SetId(&id)
displayName := "Custom application consent policy"
requestBody.SetDisplayName(&displayName)
description := "A custom permission grant policy to customize conditions for granting consent."
requestBody.SetDescription(&description)
result, err := graphClient.Policies().PermissionGrantPolicies().Post(requestBody)


```
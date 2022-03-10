---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23c074dfed9afa83cd85cab5f4b6576212fe1e51
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411564"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

trustFrameworkPolicyId := "trustFrameworkPolicy-id"
result, err := graphClient.TrustFramework().PoliciesById(&trustFrameworkPolicyId).Delete(nil)


```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db255bce325200bd4e398f38e7b8de6973e13b6e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322574"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

activityBasedTimeoutPolicyId := "activityBasedTimeoutPolicy-id"
graphClient.Policies().ActivityBasedTimeoutPoliciesById(&activityBasedTimeoutPolicyId).Delete()


```
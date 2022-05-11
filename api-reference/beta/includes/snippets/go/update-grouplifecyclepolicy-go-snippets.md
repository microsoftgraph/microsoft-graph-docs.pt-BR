---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd5a12402a898fd589513d1ef45a58740d08da1a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324073"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroupLifecyclePolicy()
groupLifetimeInDays := int32(180)
requestBody.SetGroupLifetimeInDays(&groupLifetimeInDays)
managedGroupTypes := "Selected"
requestBody.SetManagedGroupTypes(&managedGroupTypes)
alternateNotificationEmails := "admin@contoso.com"
requestBody.SetAlternateNotificationEmails(&alternateNotificationEmails)
groupLifecyclePolicyId := "groupLifecyclePolicy-id"
graphClient.GroupLifecyclePoliciesById(&groupLifecyclePolicyId).Patch(requestBody)


```
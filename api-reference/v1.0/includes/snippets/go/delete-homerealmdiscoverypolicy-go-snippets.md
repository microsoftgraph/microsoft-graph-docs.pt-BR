---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3b2022de2b0b0e88fdc8f222dd1f810aec26ddb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081868"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

homeRealmDiscoveryPolicyId := "homeRealmDiscoveryPolicy-id"
graphClient.Policies().HomeRealmDiscoveryPoliciesById(&homeRealmDiscoveryPolicyId).Delete(options)


```
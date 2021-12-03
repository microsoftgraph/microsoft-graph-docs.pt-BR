---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c70afc08220687a66d41e98e9dad88b499e4f6d6
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286711"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupLifecyclePolicyId := "groupLifecyclePolicy-id"
graphClient.GroupLifecyclePoliciesById(&groupLifecyclePolicyId).Delete(nil)


```
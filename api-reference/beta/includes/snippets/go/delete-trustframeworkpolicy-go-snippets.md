---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75ed8e8b157cecf782ea586bab16fa598be2b6fa
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287056"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

trustFrameworkPolicyId := "trustFrameworkPolicy-id"
graphClient.TrustFramework().PoliciesById(&trustFrameworkPolicyId).Delete(nil)


```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1839f2a589471f25719ca9700b9eddf0f72f6851
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286138"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

conditionalAccessPolicyId := "conditionalAccessPolicy-id"
result, err := graphClient.Identity().ConditionalAccess().PoliciesById(&conditionalAccessPolicyId).Get(nil)


```
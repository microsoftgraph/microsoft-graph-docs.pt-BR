---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8461dd1b184081040d95b7c7463785d2b2919177
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322918"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

authenticationContextClassReferenceId := "authenticationContextClassReference-id"
result, err := graphClient.Identity().ConditionalAccess().AuthenticationContextClassReferencesById(&authenticationContextClassReferenceId).Get()


```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3a883ba0aec77e5c0c1efdc6d249c1c7db2acb10
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323095"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

riskyServicePrincipalId := "riskyServicePrincipal-id"
result, err := graphClient.IdentityProtection().RiskyServicePrincipalsById(&riskyServicePrincipalId).Get()


```
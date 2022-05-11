---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 003538ffba922b10c136a449d7072d04e89ff765
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324592"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

emailAuthenticationMethodId := "emailAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().EmailMethodsById(&emailAuthenticationMethodId).Get()


```
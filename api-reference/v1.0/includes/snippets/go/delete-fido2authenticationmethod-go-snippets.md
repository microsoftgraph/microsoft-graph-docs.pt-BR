---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7e059e8b620c09c5a6bbe8a3ceb003bdb6a1c445
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322426"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
fido2AuthenticationMethodId := "fido2AuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().Fido2MethodsById(&fido2AuthenticationMethodId).Delete()


```
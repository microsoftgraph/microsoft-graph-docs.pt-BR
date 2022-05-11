---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45d8f8aa7c5c0ba5c4be22b674fed37365745871
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325036"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

phoneAuthenticationMethodId := "phoneAuthenticationMethod-id"
graphClient.Me().Authentication().PhoneMethodsById(&phoneAuthenticationMethodId).Delete()


```
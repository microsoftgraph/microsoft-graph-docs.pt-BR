---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e91199513d441cb26b7cc04a5d62f698c8e8d078
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095324"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

phoneAuthenticationMethodId := "phoneAuthenticationMethod-id"
graphClient.Me().Authentication().PhoneMethodsById(&phoneAuthenticationMethodId).Delete(options)


```
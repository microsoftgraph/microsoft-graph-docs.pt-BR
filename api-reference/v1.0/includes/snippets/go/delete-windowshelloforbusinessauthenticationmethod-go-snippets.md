---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 399cc936a765178b230b9f2411508ac5073aa859
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082563"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
windowsHelloForBusinessAuthenticationMethodId := "windowsHelloForBusinessAuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().WindowsHelloForBusinessMethodsById(&windowsHelloForBusinessAuthenticationMethodId).Delete(options)


```
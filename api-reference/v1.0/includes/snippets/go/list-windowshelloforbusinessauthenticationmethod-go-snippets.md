---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8e9fe439a7f79b21cbf681ee18b60bb2a8f113db
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082664"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).Authentication().WindowsHelloForBusinessMethods().Get(options)


```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17823e753acc26f08d02967b9de7e41a0929c932
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093162"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
temporaryAccessPassAuthenticationMethodId := "temporaryAccessPassAuthenticationMethod-id"
result, err := graphClient.UsersById(&userId).Authentication().TemporaryAccessPassMethodsById(&temporaryAccessPassAuthenticationMethodId).Get()


```
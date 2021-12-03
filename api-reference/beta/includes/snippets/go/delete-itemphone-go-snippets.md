---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9eae728e4eb4ec0ebee0fb46e84ea81c7cb90a68
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286854"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
itemPhoneId := "itemPhone-id"
graphClient.UsersById(&userId).Profile().PhonesById(&itemPhoneId).Delete(nil)


```
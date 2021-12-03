---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8ec196c924feb6d11dde5d052965c9eaa6c09abc
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286621"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userAccountInformationId := "userAccountInformation-id"
result, err := graphClient.Me().Profile().AccountById(&userAccountInformationId).Get(nil)


```
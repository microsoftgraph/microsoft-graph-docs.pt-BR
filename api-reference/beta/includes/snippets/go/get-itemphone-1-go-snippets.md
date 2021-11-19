---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c92438842150a54cfa15fa6cecf019db68a20d18
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098330"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

itemPhoneId := "itemPhone-id"
result, err := graphClient.Me().Profile().PhonesById(&itemPhoneId).Get(options)


```
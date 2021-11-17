---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5412d8cc4304a6214244e97771c824b9170ef92
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033954"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

personNameId := "personName-id"
result, err := graphClient.Me().Profile().NamesById(&personNameId).Get(options)


```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12191d5edb8e3644de5be5f45b4a3db1c230c3a7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096318"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

itemPatentId := "itemPatent-id"
result, err := graphClient.Me().Profile().PatentsById(&itemPatentId).Get(options)


```
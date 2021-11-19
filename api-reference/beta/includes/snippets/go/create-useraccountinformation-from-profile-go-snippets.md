---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8645d8e5e7f842d8b7a7e6e8453bcd89f49cd39
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103297"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Profile().Account().Post(options)


```
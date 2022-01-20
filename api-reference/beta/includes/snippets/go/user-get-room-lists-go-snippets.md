---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7e047aab43d31c88c3f781f53a7bafd03d2b2ae
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105062"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().FindRoomLists()().Get(nil)


```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3efbd789f32e259ce6adc750e56b9ed90669a739
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63527984"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
graphClient.UsersById(&userId).TransitiveReports().$count().Get(nil)


```
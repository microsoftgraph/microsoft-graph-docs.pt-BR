---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c248fa98f94cbb3d4250026ad70bc6a815d2330e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115229"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().FindRooms()().Get(nil)


```
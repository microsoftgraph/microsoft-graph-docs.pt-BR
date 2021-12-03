---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1ac796bc97ad6d48faeacc2a30d1c9419e6c15dc
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285985"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
audioRoutingGroupId := "audioRoutingGroup-id"
graphClient.Communications().CallsById(&callId).AudioRoutingGroupsById(&audioRoutingGroupId).Delete(nil)


```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f249e73aaf1977cc6361e0ca786872becba65ad3
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286517"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
shiftId := "shift-id"
graphClient.TeamsById(&teamId).Schedule().ShiftsById(&shiftId).Delete(nil)


```
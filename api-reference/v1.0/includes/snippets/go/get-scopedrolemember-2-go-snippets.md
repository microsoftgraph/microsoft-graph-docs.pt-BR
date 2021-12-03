---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 502d6b08111b622e3122694d58e9d0ff96645faf
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286316"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

administrativeUnitId := "administrativeUnit-id"
result, err := graphClient.Directory().AdministrativeUnitsById(&administrativeUnitId).ScopedRoleMembers().Get(nil)


```
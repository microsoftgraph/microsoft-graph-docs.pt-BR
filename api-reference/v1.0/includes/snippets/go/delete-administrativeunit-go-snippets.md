---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84066f102fe687fff1f605112a6bd76ba242af9f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411393"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

administrativeUnitId := "administrativeUnit-id"
result, err := graphClient.Directory().AdministrativeUnitsById(&administrativeUnitId).Delete(nil)


```
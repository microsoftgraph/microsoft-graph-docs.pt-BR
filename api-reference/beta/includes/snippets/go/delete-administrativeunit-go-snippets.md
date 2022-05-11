---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0be474e1784389ab0104dfe26bd1d65dedb0775f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322564"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

administrativeUnitId := "administrativeUnit-id"
graphClient.AdministrativeUnitsById(&administrativeUnitId).Delete()


```
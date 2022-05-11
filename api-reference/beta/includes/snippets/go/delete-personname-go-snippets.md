---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4a82b47cb816d3667205d61d007cc27683a3641
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323107"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personNameId := "personName-id"
graphClient.Me().Profile().NamesById(&personNameId).Delete()


```
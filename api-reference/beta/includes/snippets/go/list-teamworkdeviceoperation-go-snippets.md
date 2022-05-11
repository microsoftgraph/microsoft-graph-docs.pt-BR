---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6837d857dbbb8cb56c63b68abd3aef247c42a4d2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322203"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamworkDeviceId := "teamworkDevice-id"
result, err := graphClient.Teamwork().DevicesById(&teamworkDeviceId).Operations().Get()


```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c299cbdcc2d147623448f5872c2500a4c17d9393
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322939"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printConnectorId := "printConnector-id"
result, err := graphClient.Print().ConnectorsById(&printConnectorId).Get()


```
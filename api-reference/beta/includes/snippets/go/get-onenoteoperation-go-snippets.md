---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77ebae835cce2de49ffc55c2cf1de02609730b08
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325658"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onenoteOperationId := "onenoteOperation-id"
result, err := graphClient.Me().Onenote().OperationsById(&onenoteOperationId).Get()


```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 536784bf27adea90348fe182d017e051996afb31
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65629270"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

externalConnectionId := "externalConnection-id"
result, err := graphClient.External().ConnectionsById(&externalConnectionId).Get()


```
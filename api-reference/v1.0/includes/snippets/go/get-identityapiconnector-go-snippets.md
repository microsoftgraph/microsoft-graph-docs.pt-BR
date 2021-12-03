---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e14aea0d30d377132806c91bfaabfcb14944761d
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286022"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityApiConnectorId := "identityApiConnector-id"
result, err := graphClient.Identity().ApiConnectorsById(&identityApiConnectorId).Get(nil)


```
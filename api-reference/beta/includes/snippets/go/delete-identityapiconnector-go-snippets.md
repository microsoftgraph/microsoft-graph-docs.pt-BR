---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f5e819638c7d5e3289b25acfe7ec509ccfe4df65
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60998231"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

identityApiConnectorId := "identityApiConnector-id"
graphClient.Identity().ApiConnectorsById(&identityApiConnectorId).Delete(options)


```
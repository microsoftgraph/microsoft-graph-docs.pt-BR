---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4739db11ca6600f75d1b85b4d0d7ef80f5da3584
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092690"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).UnsetVerifiedPublisher().Post(options)


```
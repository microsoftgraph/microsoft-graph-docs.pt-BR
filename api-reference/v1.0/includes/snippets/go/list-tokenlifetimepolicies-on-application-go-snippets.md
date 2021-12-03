---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc99addd55d897e3c510728c5558e06737b7de9d
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287341"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).TokenLifetimePolicies().Get(nil)


```
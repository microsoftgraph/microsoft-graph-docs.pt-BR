---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5e9b315eed5905c3acfac29d375fd2fd28b84fd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322728"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).UnsetVerifiedPublisher(application-id).Post()


```
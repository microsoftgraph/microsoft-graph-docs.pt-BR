---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f064c13ee91b2b40c57bb7217b03d271b9a5749f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324509"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personCertificationId := "personCertification-id"
result, err := graphClient.Me().Profile().CertificationsById(&personCertificationId).Get()


```
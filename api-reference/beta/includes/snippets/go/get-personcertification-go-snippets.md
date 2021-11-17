---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f009e966353e999c8813f5136a50aad1c1c9d6d0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018133"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

personCertificationId := "personCertification-id"
result, err := graphClient.Me().Profile().CertificationsById(&personCertificationId).Get(options)


```
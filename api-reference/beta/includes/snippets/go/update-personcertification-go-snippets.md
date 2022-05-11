---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8cf8626f206fc62a0911da457b5eec5370107a57
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325038"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonCertification()
issuingAuthority := "International Academy of Marketing Excellence"
requestBody.SetIssuingAuthority(&issuingAuthority)
issuingCompany := "International Academy of Marketing Excellence"
requestBody.SetIssuingCompany(&issuingCompany)
userId := "user-id"
personCertificationId := "personCertification-id"
graphClient.UsersById(&userId).Profile().CertificationsById(&personCertificationId).Patch(requestBody)


```
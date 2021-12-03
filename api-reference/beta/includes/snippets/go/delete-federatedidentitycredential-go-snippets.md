---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3e8448a689b2be5d6b96ea10de71d3714fe4f8ec
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285864"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
federatedIdentityCredentialId := "federatedIdentityCredential-id"
graphClient.ApplicationsById(&applicationId).FederatedIdentityCredentialsById(&federatedIdentityCredentialId).Delete(nil)


```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79179b0218dfe548ee6ada46f294545f17fd4ac7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099486"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
federatedIdentityCredentialId := "federatedIdentityCredential-id"
result, err := graphClient.ApplicationsById(&applicationId).FederatedIdentityCredentialsById(&federatedIdentityCredentialId).Get(options)


```
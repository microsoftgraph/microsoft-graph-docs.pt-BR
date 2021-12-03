---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85b7b77091f534dc7831f0e98d945c8fba63c4ed
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286063"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

domainId := "domain-id"
result, err := graphClient.DomainsById(&domainId).VerificationDnsRecords().Get(nil)


```
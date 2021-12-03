---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 564818a657a94b66104426c9ac90b3cc71a25e88
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287320"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

domainId := "domain-id"
result, err := graphClient.DomainsById(&domainId).ServiceConfigurationRecords().Get(nil)


```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1cbc087b345df6a69a884aa3c95d647d9513f5c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030313"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

domainId := "domain-id"
result, err := graphClient.DomainsById(&domainId).ServiceConfigurationRecords().Get(options)


```
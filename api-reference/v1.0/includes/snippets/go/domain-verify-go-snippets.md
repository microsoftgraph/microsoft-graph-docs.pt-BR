---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48c9fbbb9c954acd4f26afe341985bfe11dc70ee
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324493"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

domainId := "domain-id"
result, err := graphClient.DomainsById(&domainId).Verify(domain-id).Post()


```
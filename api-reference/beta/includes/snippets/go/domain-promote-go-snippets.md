---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa2055bd8ef81f1bd56bb09ee771f2c9f0ad9e5c
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "66446575"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

domainId := "domain-id"
result, err := graphClient.DomainsById(&domainId).Promote(domain-id).Post()


```
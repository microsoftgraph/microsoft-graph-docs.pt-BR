---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1139ddcfb56f7e881877e56ff3aa9c8e7d962fb
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287281"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

domainId := "domain-id"
result, err := graphClient.DomainsById(&domainId).DomainNameReferences().Get(nil)


```
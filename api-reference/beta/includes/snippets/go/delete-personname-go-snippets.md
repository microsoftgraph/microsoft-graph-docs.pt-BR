---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 80bed4cdebd3d43cf477dee5f4e9bcc3fddecccf
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286041"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personNameId := "personName-id"
graphClient.Me().Profile().NamesById(&personNameId).Delete(nil)


```
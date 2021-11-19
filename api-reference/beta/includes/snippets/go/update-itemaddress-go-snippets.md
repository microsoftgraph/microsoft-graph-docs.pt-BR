---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1eb353156e8830cdf6dd7f40e15627ee5ddca3a5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102766"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
itemAddressId := "itemAddress-id"
graphClient.UsersById(&userId).Profile().AddressesById(&itemAddressId).Patch(options)


```
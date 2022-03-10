---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a12f911d08d2dac9412854b07f609f6102490b9c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411155"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
itemAddressId := "itemAddress-id"
result, err := graphClient.UsersById(&userId).Profile().AddressesById(&itemAddressId).Delete(nil)


```
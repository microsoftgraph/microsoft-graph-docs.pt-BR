---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95199b6292ee11322307bb3c03f03f8a666a4050
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286443"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedAccessId := "privilegedAccess-id"
result, err := graphClient.PrivilegedAccessById(&privilegedAccessId).Resources().Get(nil)


```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1183ae7aa10592340f10b22b357d2188418516c5
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286502"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Authentication().PasswordlessMicrosoftAuthenticatorMethods().Get(nil)


```
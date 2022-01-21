---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 128deb64bac2e8f063598482793c90660465d5f8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62093238"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().GetCredentialUserRegistrationCount()().Get(nil)


```
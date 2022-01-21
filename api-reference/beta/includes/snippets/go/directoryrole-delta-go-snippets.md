---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0ec75563a2e3e3439c7901a47f46ad9a14826e1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137476"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.DirectoryRoles().Delta()().Get(nil)


```
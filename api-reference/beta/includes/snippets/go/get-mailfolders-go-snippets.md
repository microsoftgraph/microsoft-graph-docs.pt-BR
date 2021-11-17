---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 615de736e8d83b787496694b4a3ec3a61be91eed
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985190"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().MailFolders().Get(options)


```
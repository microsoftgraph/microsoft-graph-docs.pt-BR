---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4228de41e766eb6de2cebbb2fa93876f1351eac
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017398"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

setId := "set-id"
graphClient.TermStore().SetsById(&setId).Delete(options)


```
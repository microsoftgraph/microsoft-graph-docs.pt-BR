---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f251da75eeafba3b6ceb174da85d72bbb8663928
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322343"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directoryAuditId := "directoryAudit-id"
result, err := graphClient.AuditLogs().DirectoryAuditsById(&directoryAuditId).Get()


```
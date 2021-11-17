---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 388208761e381691bae44f20de86c3480c46e342
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015641"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

directorySettingTemplateId := "directorySettingTemplate-id"
result, err := graphClient.DirectorySettingTemplatesById(&directorySettingTemplateId).Get(options)


```
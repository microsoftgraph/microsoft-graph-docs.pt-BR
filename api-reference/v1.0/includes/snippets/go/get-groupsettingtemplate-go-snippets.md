---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1dd523f437be325734210df79c274f7292ad8bea
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325199"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupSettingTemplateId := "groupSettingTemplate-id"
result, err := graphClient.GroupSettingTemplatesById(&groupSettingTemplateId).Get()


```
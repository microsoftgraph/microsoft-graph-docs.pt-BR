---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7282aeb38405680450077ba0c65edb6907962c8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323044"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewColumnDefinition()
description := "test"
requestBody.SetDescription(&description)
enforceUniqueValues := false
requestBody.SetEnforceUniqueValues(&enforceUniqueValues)
hidden := false
requestBody.SetHidden(&hidden)
indexed := false
requestBody.SetIndexed(&indexed)
name := "Title"
requestBody.SetName(&name)
text := msgraphsdk.NewTextColumn()
requestBody.SetText(text)
allowMultipleLines := false
text.SetAllowMultipleLines(&allowMultipleLines)
appendChangesToExistingText := false
text.SetAppendChangesToExistingText(&appendChangesToExistingText)
linesForEditing := int32(0)
text.SetLinesForEditing(&linesForEditing)
maxLength := int32(255)
text.SetMaxLength(&maxLength)
siteId := "site-id"
result, err := graphClient.SitesById(&siteId).Columns().Post(requestBody)


```
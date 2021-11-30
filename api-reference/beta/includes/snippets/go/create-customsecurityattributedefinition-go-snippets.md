---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb51335bcf7139637e73c8df0322180f3cd1f359
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226774"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCustomSecurityAttributeDefinition()
attributeSet := "Engineering"
requestBody.SetAttributeSet(&attributeSet)
description := "Target completion date"
requestBody.SetDescription(&description)
isCollection := false
requestBody.SetIsCollection(&isCollection)
isSearchable := true
requestBody.SetIsSearchable(&isSearchable)
name := "ProjectDate"
requestBody.SetName(&name)
status := "Available"
requestBody.SetStatus(&status)
type := "String"
requestBody.SetType(&type)
usePreDefinedValuesOnly := false
requestBody.SetUsePreDefinedValuesOnly(&usePreDefinedValuesOnly)
options := &msgraphsdk.CustomSecurityAttributeDefinitionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Directory().CustomSecurityAttributeDefinitions().Post(options)


```
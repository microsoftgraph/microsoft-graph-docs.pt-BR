---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acf4f5a262d6d3c74a0fc9e0b596e99d514895b3
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226777"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCustomSecurityAttributeDefinition()
attributeSet := "Engineering"
requestBody.SetAttributeSet(&attributeSet)
description := "Active projects for user"
requestBody.SetDescription(&description)
isCollection := true
requestBody.SetIsCollection(&isCollection)
isSearchable := true
requestBody.SetIsSearchable(&isSearchable)
name := "Project"
requestBody.SetName(&name)
status := "Available"
requestBody.SetStatus(&status)
type := "String"
requestBody.SetType(&type)
usePreDefinedValuesOnly := true
requestBody.SetUsePreDefinedValuesOnly(&usePreDefinedValuesOnly)
options := &msgraphsdk.CustomSecurityAttributeDefinitionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Directory().CustomSecurityAttributeDefinitions().Post(options)


```
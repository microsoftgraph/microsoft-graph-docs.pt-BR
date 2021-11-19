---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2825c2f7321f82e8243e96df63c6fbb6f9c957f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097772"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSchemaExtension()
id := "graphlearn_courses"
requestBody.SetId(&id)
description := "Graph Learn training courses extensions"
requestBody.SetDescription(&description)
requestBody.SetTargetTypes( []String {
    "Group",
}
requestBody.SetProperties( []ExtensionSchemaProperty {
    msgraphsdk.NewExtensionSchemaProperty(),
    SetAdditionalData(map[string]interface{}{
        "name": "courseId",
        "type": "Integer",
    }
    msgraphsdk.NewExtensionSchemaProperty(),
    SetAdditionalData(map[string]interface{}{
        "name": "courseName",
        "type": "String",
    }
    msgraphsdk.NewExtensionSchemaProperty(),
    SetAdditionalData(map[string]interface{}{
        "name": "courseType",
        "type": "String",
    }
}
options := &msgraphsdk.SchemaExtensionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.SchemaExtensions().Post(options)


```
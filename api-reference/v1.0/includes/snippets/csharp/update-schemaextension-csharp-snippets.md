---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21967c953ad194a4457a3a4d20b0bc4bf0b2a011e78e889d93987bf6528dfc37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272161"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtension = new SchemaExtension
{
    Properties = new List<ExtensionSchemaProperty>()
    {
        new ExtensionSchemaProperty
        {
            Name = "new-name-value",
            Type = "new-type-value"
        },
        new ExtensionSchemaProperty
        {
            Name = "additional-name-value",
            Type = "additional-type-value"
        }
    }
};

await graphClient.SchemaExtensions["{schemaExtension-id}"]
    .Request()
    .UpdateAsync(schemaExtension);

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8228e07c9da540665615b98064712514a44cc0d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978728"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SchemaExtension schemaExtension = new SchemaExtension();
LinkedList<ExtensionSchemaProperty> propertiesList = new LinkedList<ExtensionSchemaProperty>();
ExtensionSchemaProperty properties = new ExtensionSchemaProperty();
properties.name = "new-name-value";
properties.type = "new-type-value";
propertiesList.add(properties);
ExtensionSchemaProperty properties1 = new ExtensionSchemaProperty();
properties1.name = "additional-name-value";
properties1.type = "additional-type-value";
propertiesList.add(properties1);
schemaExtension.properties = propertiesList;

graphClient.schemaExtensions("{id}")
    .buildRequest()
    .patch(schemaExtension);

```
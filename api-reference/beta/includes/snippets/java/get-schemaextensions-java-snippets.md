---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58a55db53668da84accc1d5b8d9dece51613bcb7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870638"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$filter", "id eq 'graphlearn_test'"));

ISchemaExtensionCollectionPage schemaExtensions = graphClient.schemaExtensions()
    .buildRequest( requestOptions )
    .get();

```
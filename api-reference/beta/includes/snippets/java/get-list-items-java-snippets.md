---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7512147f5e7e39aaef6346268b4cc26f8c606b71
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971329"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "fields(select=Name,Color,Quantity)"));

IListItemCollectionPage items = graphClient.sites("{site-id}").lists("{list-id}").items()
    .buildRequest( requestOptions )
    .get();

```
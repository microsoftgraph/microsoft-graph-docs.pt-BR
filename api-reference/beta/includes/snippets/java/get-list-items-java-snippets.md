---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7512147f5e7e39aaef6346268b4cc26f8c606b71
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880185"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "fields(select=Name,Color,Quantity)"));

IListItemCollectionPage items = graphClient.sites("{site-id}").lists("{list-id}").items()
    .buildRequest( requestOptions )
    .get();

```
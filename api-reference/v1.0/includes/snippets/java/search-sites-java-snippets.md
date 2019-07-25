---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e3449077169acc018398759cb86195106cbf1f64
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892210"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("search", "{query}"));

ISiteCollectionPage sites = graphClient.sites()
    .buildRequest( requestOptions )
    .get();

```
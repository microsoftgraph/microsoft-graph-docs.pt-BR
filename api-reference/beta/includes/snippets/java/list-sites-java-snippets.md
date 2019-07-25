---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1d329dfb72db0a7ad386976d54e3f9146754cc7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869627"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("select", "siteCollection,webUrl"));
requestOptions.add(new QueryOption("filter", "siteCollection/root ne null"));
requestOptions.add(new QueryOption("$filter", "siteCollection/root ne null"));

ISiteCollectionPage sites = graphClient.sites()
    .buildRequest( requestOptions )
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7b7813c4f6bb003612cbc4811f97f8b3d87fe9dd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858186"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$filter", "hasMembersWithLicenseErrors+eq+true,"));

IGroupCollectionPage groups = graphClient.groups()
    .buildRequest( requestOptions )
    .select("id,displayName")
    .get();

```
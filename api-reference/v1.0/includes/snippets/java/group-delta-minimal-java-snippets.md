---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d7825466141c281a430f9276735d3c151ca994e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890813"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=minimal"));

IGroupDeltaCollectionPage delta = graphClient.groups()
    .delta()
    .buildRequest( requestOptions )
    .select("displayName,description,mailNickname")
    .get();

```
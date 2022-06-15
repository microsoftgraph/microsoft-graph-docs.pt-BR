---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65144dfd8f6fa6385011020bf38cb2b890102f5f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093599"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryFileCollectionPage files = graphClient.security().cases().ediscoveryCases("58399dff-cebe-478f-b1af-d3227f1fd645").reviewSets("273f11a1-17aa-419c-981d-ff10d33e420f").files()
    .buildRequest()
    .top(5)
    .get();

```
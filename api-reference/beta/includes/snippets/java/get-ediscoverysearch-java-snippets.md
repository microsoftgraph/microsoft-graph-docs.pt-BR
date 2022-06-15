---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28a6d9c6239f9871b0269e69b1404cb059717281
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093095"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoverySearch ediscoverySearch = graphClient.security().cases().ediscoveryCases("58399dff-cebe-478f-b1af-d3227f1fd645").searches("60150269-9758-4439-9bc4-453c864d082f")
    .buildRequest()
    .get();

```
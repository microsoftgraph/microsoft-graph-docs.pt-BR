---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 394aa07e2f682408263b6f4e941263e1e66eea3f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968445"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveSearchCollectionPage search = graphClient.me().drive()
    .search(DriveSearchParameterSet
        .newBuilder()
        .withQ("Contoso Project")
        .build())
    .buildRequest()
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24ea076513d2a905bb22a31efa7cc21034ea7b0f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975851"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveCollectionPage drives = graphClient.me().drives()
    .buildRequest()
    .get();

```
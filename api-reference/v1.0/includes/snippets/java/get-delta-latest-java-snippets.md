---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a31b95347f105875a95f3fa2bb51e6db6c6a2505ab98e7d366824473e37ea8ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100279"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("token", "latest"));

DriveItemDeltaCollectionPage delta = graphClient.me().drive().root()
    .delta()
    .buildRequest( requestOptions )
    .get();

```
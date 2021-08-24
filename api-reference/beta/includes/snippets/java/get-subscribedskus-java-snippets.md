---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 548f14df40611f4795b4060cb1050901fe8179c2cd99529d7299a9bc574eb357
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102064"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SubscribedSkuCollectionPage subscribedSkus = graphClient.subscribedSkus()
    .buildRequest()
    .get();

```
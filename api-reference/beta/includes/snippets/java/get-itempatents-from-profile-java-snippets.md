---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0bb64fc5bdd2f0bca11ad9b622aa10be9b47d3dc98cb7455eb6dd50309166356
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159194"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPatentCollectionPage patents = graphClient.me().profile().patents()
    .buildRequest()
    .get();

```
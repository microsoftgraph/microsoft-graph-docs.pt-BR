---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4d56867551f1c45d5e554b85b9ec46ea6990a1a1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976973"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedResource linkedResource = new LinkedResource();
linkedResource.webUrl = "https://microsoft.com";
linkedResource.applicationName = "Microsoft";
linkedResource.displayName = "Microsoft";
linkedResource.externalId = "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9";

graphClient.me().todo().lists("dfsdc-f9dfdfs-dcsda9").tasks("e2dc-f9cce2-dce29").linkedResources()
    .buildRequest()
    .post(linkedResource);

```
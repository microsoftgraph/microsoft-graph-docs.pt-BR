---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c615af75755408becc42fc800ce391bbcd82f92be1ecac2e3d72801822f97921
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375909"
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
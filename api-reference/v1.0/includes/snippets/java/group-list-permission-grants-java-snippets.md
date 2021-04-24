---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5df4b986513954810962a11b4949f50d519ea67f
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961385"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ResourceSpecificPermissionGrantCollectionPage permissionGrants = graphClient.groups("14c981a4-dca9-4565-bae6-e13ada8861be").permissionGrants()
    .buildRequest()
    .get();

```
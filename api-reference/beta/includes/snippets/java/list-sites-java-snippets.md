---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7036f7fb8e78ea8ce8616784a6764519cdb87a32e37541fd93ad757e14f2ba1f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216665"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteCollectionPage sites = graphClient.sites()
    .buildRequest()
    .filter("siteCollection/root ne null")
    .select("siteCollection,webUrl")
    .get();

```
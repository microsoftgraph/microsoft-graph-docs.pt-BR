---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2f0fed934fff9222b7919a3cc1003d67b63fbdbf52e2e145d886aa6ac4b66da9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159890"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

VirtualEndpointGetEffectivePermissionsCollectionPage getEffectivePermissions = graphClient.deviceManagement().virtualEndpoint()
    .getEffectivePermissions()
    .buildRequest()
    .get();

```
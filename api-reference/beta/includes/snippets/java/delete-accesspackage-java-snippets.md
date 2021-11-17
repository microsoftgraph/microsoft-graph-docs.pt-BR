---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48f36ce1254b41585eb2aa891e5d911c7ae1940a83ef56e6f21b089ad15e6dc8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099904"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackages("{id}")
    .buildRequest()
    .delete();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ab965cc2ecc17da90f1b1e7ad3bd9947d13bd02151c9bf9cccd640855c17285
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216151"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecurityActionCollectionPage securityActions = graphClient.security().securityActions()
    .buildRequest()
    .get();

```
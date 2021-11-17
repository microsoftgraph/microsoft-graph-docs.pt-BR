---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1c17430e47453526ce2ab69b2addee52606eae927dc5a3336e00b78b9766d315
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157112"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectedOrganization connectedOrganization = graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{id}")
    .buildRequest()
    .get();

```
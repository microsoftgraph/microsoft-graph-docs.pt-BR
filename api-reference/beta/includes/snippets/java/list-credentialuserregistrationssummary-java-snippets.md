---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3b1b34e73ecdcb73d49f8ed352f54e80d681ed2263fb2de331dfdec5a7377a09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273319"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CredentialUserRegistrationsSummaryCollectionPage credentialUserRegistrationsSummaries = graphClient.tenantRelationships().managedTenants().credentialUserRegistrationsSummaries()
    .buildRequest()
    .get();

```
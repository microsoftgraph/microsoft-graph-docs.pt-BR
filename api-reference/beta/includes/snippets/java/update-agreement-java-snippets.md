---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20595ed7f70478f53484f53261ac07ba40ea63e3350737ec53713486d240a01b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898051"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Agreement agreement = new Agreement();
agreement.displayName = "displayName-value";
agreement.isViewingBeforeAcceptanceRequired = true;

graphClient.identityGovernance().termsOfUse().agreements("{id}")
    .buildRequest()
    .patch(agreement);

```
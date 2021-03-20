---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce43a7ae39504b5b72e5f7603950d7b51d2a8097
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975777"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("{id}")
    .buildRequest()
    .delete();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7d660d620c97c843acac7ad673a7700d68b6123730b1de3aac92ae327e3e0842
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099888"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCollectionPage accessPackages = graphClient.identityGovernance().entitlementManagement().accessPackages()
    .buildRequest()
    .get();

```
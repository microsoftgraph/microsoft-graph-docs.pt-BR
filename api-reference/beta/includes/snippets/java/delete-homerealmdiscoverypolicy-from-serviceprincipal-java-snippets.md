---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 446c78bb70857e7bdc12785f5703d692aaa08e3546fd420724c5ea6301932aa1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101952"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{servicePrincipalId}").homeRealmDiscoveryPolicies("{policyId}").reference()
    .buildRequest()
    .delete();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 024cb8cce84fbe074fe94779fc02fd44e555ad0bcdb622c110416221c7979d6c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158205"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcProvisioningPolicyCollectionPage provisioningPolicies = graphClient.deviceManagement().virtualEndpoint().provisioningPolicies()
    .buildRequest()
    .get();

```
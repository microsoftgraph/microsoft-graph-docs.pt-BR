---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cbcdbf60f26c2704744d1907017283817ed7cec5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976820"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcProvisioningPolicy cloudPcProvisioningPolicy = new CloudPcProvisioningPolicy();
cloudPcProvisioningPolicy.displayName = "Display Name value";
cloudPcProvisioningPolicy.description = "Description value";
cloudPcProvisioningPolicy.onPremisesConnectionId = "6bf90392-5fea-459a-9e9d-a2484abbffff";
cloudPcProvisioningPolicy.imageId = "Image ID value";
cloudPcProvisioningPolicy.imageDisplayName = "Image Display Name value";
cloudPcProvisioningPolicy.imageType = CloudPcProvisioningPolicyImageType.GALLERY;

graphClient.deviceManagement().virtualEndpoint().provisioningPolicies()
    .buildRequest()
    .post(cloudPcProvisioningPolicy);

```
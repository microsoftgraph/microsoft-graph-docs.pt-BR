---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 049824afbaf190b7e2d63a21293179fe63844177
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225085"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcUserAccountType userAccountType = CloudPcUserAccountType.ADMINISTRATOR;

CloudPcOperatingSystem osVersion = CloudPcOperatingSystem.WINDOWS10;

graphClient.deviceManagement().virtualEndpoint().cloudPCs("4b5ad5e0-6a0b-4ffc-818d-36bb23cf4dbd")
    .reprovision(CloudPCReprovisionParameterSet
        .newBuilder()
        .withUserAccountType(userAccountType)
        .withOsVersion(osVersion)
        .build())
    .buildRequest()
    .post();

```
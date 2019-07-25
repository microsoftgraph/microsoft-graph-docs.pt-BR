---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39ec9865f613bccce16a21f8128ae5126ad16574
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870244"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecurityAction securityAction = new SecurityAction();
securityAction.name = "BlockIp";
securityAction.actionReason = "Test";
LinkedList<KeyValuePair> parametersList = new LinkedList<KeyValuePair>();
KeyValuePair parameters = new KeyValuePair();
parameters.name = "IP";
parameters.value = "1.2.3.4";
parametersList.add(parameters);
securityAction.parameters = parametersList;
SecurityVendorInformation vendorInformation = new SecurityVendorInformation();
vendorInformation.provider = "Windows Defender ATP";
vendorInformation.vendor = "Microsoft";
securityAction.vendorInformation = vendorInformation;

graphClient.security().securityActions()
    .buildRequest()
    .post(securityAction);

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5ca180f89f57446bfea94c7124c27b7a222ad697
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224498"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AllowedValue allowedValue = new AllowedValue();
allowedValue.id = "Alpine";
allowedValue.isActive = false;

graphClient.directory().customSecurityAttributeDefinitions("Engineering_Project").allowedValues()
    .buildRequest()
    .post(allowedValue);

```
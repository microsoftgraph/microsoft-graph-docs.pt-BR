---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d220ffeea84c8cb799e2e2385b3531e57026d2f0
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225939"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AllowedValueCollectionPage allowedValues = graphClient.directory().customSecurityAttributeDefinitions("Engineering_Project").allowedValues()
    .buildRequest()
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75cedf7603d26f12ce25a2992f3f8bb7ef048fd2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315655"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalDomainNameCollectionPage domains = graphClient.directory().federationConfigurations().microsoft.graph.samlOrWsFedExternalDomainFederation("f1e11a04-0244-4592-99df-b01cfaadce15").domains()
    .buildRequest()
    .get();

```
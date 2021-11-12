---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7d7d92ee2e0bf4973943a353918ca705d55df8bff8220b5c5a565860f313bfa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100487"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DomainDnsRecordCollectionPage verificationDnsRecords = graphClient.domains("contoso.com").verificationDnsRecords()
    .buildRequest()
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0c0b24afc7b47599b10ade8f2fb0176edde46081425e747995c4bf0ddeee7bd2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103050"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DomainDnsRecordCollectionPage verificationDnsRecords = graphClient.domains("{domain-name}").verificationDnsRecords()
    .buildRequest()
    .get();

```
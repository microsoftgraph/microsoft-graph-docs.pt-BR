---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6849b73e6b585d4e0ac2e5d16c65a47dbf0a48b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968796"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DomainDnsRecordCollectionPage serviceConfigurationRecords = graphClient.domains("{domain-name}").serviceConfigurationRecords()
    .buildRequest()
    .get();

```
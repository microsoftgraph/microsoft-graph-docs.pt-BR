---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4cba3ab307374904a725559153f6ebc0cb2748f6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889905"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDomainDnsRecordCollectionPage serviceConfigurationRecords = graphClient.domains("{domain-name}").serviceConfigurationRecords()
    .buildRequest()
    .get();

```
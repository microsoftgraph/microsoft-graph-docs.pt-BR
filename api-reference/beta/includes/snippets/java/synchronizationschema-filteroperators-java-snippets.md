---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17f0887efc21605e626b90b92e3a8fec44b23832b2d1b6324bb4db941be32f61
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100148"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationSchemaFilterOperatorsCollectionPage filterOperators = graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}").schema()
    .filterOperators()
    .buildRequest()
    .get();

```
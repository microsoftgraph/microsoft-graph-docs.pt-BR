---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13bdf62b094c686e0d1b9cfd97a9a3f8dccac646
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955833"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveCollectionPage drives = graphClient.sites("{siteId}").drives()
    .buildRequest()
    .get();

```
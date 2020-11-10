---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 493dd3a304b11cc0e43355722db99e739a636767
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955831"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveCollectionPage drives = graphClient.users("{userId}").drives()
    .buildRequest()
    .get();

```
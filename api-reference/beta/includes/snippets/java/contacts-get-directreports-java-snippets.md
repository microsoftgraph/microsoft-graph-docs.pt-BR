---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10b2682804eb8eb7e69d718fdf65a17629fe25ab
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975165"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage directReports = graphClient.contacts("{id}").directReports()
    .buildRequest()
    .get();

```
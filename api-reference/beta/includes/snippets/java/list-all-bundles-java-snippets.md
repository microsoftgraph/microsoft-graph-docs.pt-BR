---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8a82b4cb8d9eefd02d60b944433f5adf75f5fd2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960240"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage bundles = graphClient.drive().bundles()
    .buildRequest()
    .get();

```
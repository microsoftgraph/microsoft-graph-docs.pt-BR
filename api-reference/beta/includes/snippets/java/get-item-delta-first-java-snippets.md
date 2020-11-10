---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b38bda8a978c8ebfcd0878af28fcebe69bfa1398
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963802"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemDeltaCollectionPage delta = graphClient.me().drive().root()
    .delta()
    .buildRequest()
    .get();

```
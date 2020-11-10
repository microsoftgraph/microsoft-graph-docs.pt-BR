---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 362864f5d4805d68ba312af24e0d1a44bc67cef7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955727"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveRecentCollectionPage recent = graphClient.me().drive()
    .recent()
    .buildRequest()
    .get();

```
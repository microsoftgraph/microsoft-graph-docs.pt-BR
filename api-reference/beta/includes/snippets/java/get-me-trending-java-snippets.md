---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f157dcbb52c36acf3bd5a6a0bd135e01569e5bd2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964632"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITrendingCollectionPage trending = graphClient.me().insights().trending()
    .buildRequest()
    .get();

```
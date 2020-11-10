---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62168004d4ed49aaa44f1d7db181c953bc1cfa61
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955865"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage following = graphClient.me().drive().following()
    .buildRequest()
    .get();

```
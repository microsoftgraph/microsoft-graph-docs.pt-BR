---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62168004d4ed49aaa44f1d7db181c953bc1cfa61
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124326"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage following = graphClient.me().drive().following()
    .buildRequest()
    .get();

```
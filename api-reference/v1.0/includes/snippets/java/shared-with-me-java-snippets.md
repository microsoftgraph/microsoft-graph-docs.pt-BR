---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4d624f6acad61fa494a75cc9d5012b22fadc5e8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983617"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveSharedWithMeCollectionPage sharedWithMe = graphClient.me().drive()
    .sharedWithMe()
    .buildRequest()
    .get();

```
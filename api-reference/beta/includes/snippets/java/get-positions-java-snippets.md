---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 665a09b9790a15129f465890a9ab2ef76972eca1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964086"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkPositionCollectionPage positions = graphClient.me().profile().positions()
    .buildRequest()
    .get();

```
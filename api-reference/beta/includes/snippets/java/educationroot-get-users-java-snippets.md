---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b33918fa2cc13222ee3b37b3311704353559766d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966087"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationUserCollectionPage users = graphClient.education().users()
    .buildRequest()
    .get();

```
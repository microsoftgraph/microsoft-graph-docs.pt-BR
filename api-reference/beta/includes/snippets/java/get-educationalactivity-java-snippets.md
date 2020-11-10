---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bfaba27c810394ddc8194faf4b6e7102acd86a81
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966660"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationalActivity educationalActivity = graphClient.me().profile().educationalActivities("{id}")
    .buildRequest()
    .get();

```
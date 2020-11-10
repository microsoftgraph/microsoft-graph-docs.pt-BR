---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fad918194947b5bf77743cf84d9ca052bc85ed51
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978168"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISynchronizationTemplateCollectionPage templates = graphClient.servicePrincipals("{id}").synchronization().templates()
    .buildRequest()
    .get();

```
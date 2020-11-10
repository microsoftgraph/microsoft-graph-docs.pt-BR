---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7fd44ff55634340b2b0d9ede03fd05f4d6d67d62
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971294"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISectionGroupCollectionPage sectionGroups = graphClient.me().onenote().notebooks("{id}").sectionGroups()
    .buildRequest()
    .get();

```
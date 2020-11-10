---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1f6b638425ea84ded4785870b6501871a30e305
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979464"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage memberOf = graphClient.users("{id}").memberOf()
    .buildRequest()
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 786c46f077dc94db4c88e153f6db27bf2c90f425
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953854"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage rejectedSenders = graphClient.groups("{id}").rejectedSenders()
    .buildRequest()
    .get();

```
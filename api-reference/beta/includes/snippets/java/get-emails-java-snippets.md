---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8041ca0cd0cb0cea12cf7a94ced8b7f7ef2a3ba4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980815"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IItemEmailCollectionPage emails = graphClient.me().profile().emails()
    .buildRequest()
    .get();

```
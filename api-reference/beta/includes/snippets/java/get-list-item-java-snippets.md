---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb6ba3551451b24e4d42e184c53392ded85991d7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971357"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "fields"));

ListItem listItem = graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}")
    .buildRequest( requestOptions )
    .get();

```
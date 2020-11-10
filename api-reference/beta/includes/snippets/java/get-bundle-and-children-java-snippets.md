---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27d0589acf573cd775b59388cd90ec2f47fdf84e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960285"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "children"));

DriveItem driveItem = graphClient.drive().items("{bundle-id}")
    .buildRequest( requestOptions )
    .get();

```
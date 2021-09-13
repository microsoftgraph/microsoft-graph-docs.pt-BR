---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8822652eb37a7dcde8b4bf060ca594bdc30c57ee363f656c7a0564d85d2accfd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899509"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

graphClient.planner().plans("{id}")
    .buildRequest( requestOptions )
    .delete();

```
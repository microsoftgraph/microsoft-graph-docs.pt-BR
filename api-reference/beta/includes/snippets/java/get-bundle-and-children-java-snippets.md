---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48a00ef5ead425fd4c274aa2e43654b8049d19223e5cda40aae6b43309c0e1b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899693"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "children"));

DriveItem driveItem = graphClient.drive().items("{bundle-id}")
    .buildRequest( requestOptions )
    .get();

```
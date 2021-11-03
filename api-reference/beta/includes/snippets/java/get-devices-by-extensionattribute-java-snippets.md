---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24214d05820c4cf8be85a3d0b15331e7136d2920
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694544"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

DeviceCollectionPage devices = graphClient.devices()
    .buildRequest( requestOptions )
    .filter("extensionAttributes/extensionAttribute1 eq 'BYOD-Device'")
    .get();

```
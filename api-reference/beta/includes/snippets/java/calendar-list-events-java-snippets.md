---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 411c32ef3f10c0b17596da1a9eeab9080ef55154
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996083"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EventCollectionPage events = graphClient.me().calendar().events()
    .buildRequest()
    .filter("startsWith(subject,'All')")
    .get();

```
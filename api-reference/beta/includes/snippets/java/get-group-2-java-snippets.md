---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 50ec9c801c347346c92978e81c60f5ed3116484a395bbc998bf7fec750011317
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101685"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionPage groups = graphClient.termStore().groups()
    .buildRequest()
    .get();

```
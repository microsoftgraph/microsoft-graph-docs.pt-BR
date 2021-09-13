---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3cb767e6239b73939a80e597aeda002d26fdd3471931fe7585b8667bc3aa14f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275310"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ListItemVersionCollectionPage versions = graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}").versions()
    .buildRequest()
    .get();

```
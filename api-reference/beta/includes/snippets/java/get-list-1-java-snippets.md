---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4daf8dcf54ca908d4fd472870d23430708250c22
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209441"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

List list = graphClient.sites("{site-id}").lists("{list-id}")
    .buildRequest()
    .get();

```
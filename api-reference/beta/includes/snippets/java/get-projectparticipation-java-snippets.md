---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6d0855aba98a166f3b84b7aa7d3af31a58cec1684748689813ea9514110b198
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156917"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProjectParticipation projectParticipation = graphClient.me().profile().projects("{id}")
    .buildRequest()
    .get();

```
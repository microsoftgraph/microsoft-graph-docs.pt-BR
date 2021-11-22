---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4cf2ae07d1e8064b0712a7721b9faddc730407732eb0c2cbdb6c0934eb68b69
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274915"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemEmail itemEmail = graphClient.users("{userId}").profile().emails("{id}")
    .buildRequest()
    .get();

```
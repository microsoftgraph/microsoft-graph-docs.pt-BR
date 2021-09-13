---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63dceb3798e821b292a3b2999b6092e260023dccd09f43fbb0eee5836433f3b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102986"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .send()
    .buildRequest()
    .post();

```
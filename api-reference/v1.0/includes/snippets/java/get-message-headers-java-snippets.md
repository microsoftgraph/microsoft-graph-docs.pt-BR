---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2548845cbbe9200d16e6ba10096d7d3083aefc4b19045ed429eef6c5e9316a95
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159482"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADhAAAW-VPeAAA=")
    .buildRequest()
    .select("internetMessageHeaders")
    .get();

```
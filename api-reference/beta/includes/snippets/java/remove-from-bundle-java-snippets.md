---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c617db22484f8691b3edc79040cc0b038c6dbc9527aa1188dc8743516f54459d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157948"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().bundles("{bundle-id}").children("{item-id}")
    .buildRequest()
    .delete();

```
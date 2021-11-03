---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3a3fcb430bbf2226d78e18fc441a7456096cf86ce4c17e1d19bfd4ed49072ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157422"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{site-id}").contentTypes("{contentType-id}").columns("{column-id}")
    .buildRequest()
    .delete();

```
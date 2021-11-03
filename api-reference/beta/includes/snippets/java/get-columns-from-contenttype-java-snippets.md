---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5a34945fcff623a25b3a9d46f5e2afca2628f350cfc7bd6ece849905c7ce3ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216986"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ColumnDefinitionCollectionPage columns = graphClient.sites("{site-id}").contentTypes("{contentType-id}").columns()
    .buildRequest()
    .get();

```
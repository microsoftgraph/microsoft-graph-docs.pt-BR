---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 627b0f43a926eaa86b04bcbc588b5553e48e6ea8e984535e450a333236955218
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159830"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ListCollectionPage lists = graphClient.sites("{site-id}").lists()
    .buildRequest()
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb094bba85e35e1aef4e57f9d86b59ce00c05fc1420e3e44fb36ea5d2f5ff28c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272134"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String string = graphClient.compliance().ediscovery().cases("99e865fc-e29f-479a-ba83-9e58eb017103").operations("63926d4779c243458902328d83f61f53").microsoft.graph.ediscovery.caseExportOperation()
    .getDownloadUrl()
    .buildRequest()
    .get();

```
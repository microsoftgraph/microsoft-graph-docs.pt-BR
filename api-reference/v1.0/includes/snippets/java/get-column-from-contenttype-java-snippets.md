---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f26c3875bf977c10f51f3c3612af9b2f382d3229
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080148"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ColumnDefinition columnDefinition = graphClient.sites("{site-id}").contentTypes("{contentType-id}").columns("{column-id}")
    .buildRequest()
    .get();

```
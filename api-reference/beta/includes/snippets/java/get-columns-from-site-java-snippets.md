---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0520be8dcc9a9e6dd27c0297bdfb9c1e9075678
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200770"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ColumnDefinitionCollectionPage columns = graphClient.sites("{site-id}").columns()
    .buildRequest()
    .get();

```
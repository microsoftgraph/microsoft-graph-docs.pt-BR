---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e16a5c23dec08282ea2d5f5cc1c8dd9ab69ab818
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208657"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Term term = graphClient.termStore().groups("{groupId}").sets("{setId}").terms("{termId}")
    .buildRequest()
    .get();

```
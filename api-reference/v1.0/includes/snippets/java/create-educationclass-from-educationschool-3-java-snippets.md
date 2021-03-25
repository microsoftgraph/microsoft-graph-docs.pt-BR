---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6cdc11e1bb9724260bbb4d53ce51de66d028cad
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209857"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("{school-id}").classes("{class-id}")
    .buildRequest()
    .delete();

```
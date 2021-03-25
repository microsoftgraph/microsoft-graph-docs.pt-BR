---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 351bafc5fbc873abb9916d5096db95b6131e5baf
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209958"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11014").assignmentCategories("19002")
    .buildRequest()
    .delete();

```
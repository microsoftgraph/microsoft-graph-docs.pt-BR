---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65c9921d3b117a2acb8cdcaad856781c3b567d73416a85a5f79dab8ec260d009
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327330"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11021").assignments("19002").submissions("850f51b7").resources("f2387c3b-ec39-4bf2-a399-d7242677f024")
    .buildRequest()
    .delete();

```
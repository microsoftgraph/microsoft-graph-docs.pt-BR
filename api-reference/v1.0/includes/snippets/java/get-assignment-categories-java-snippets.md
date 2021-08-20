---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53d10bf86d1eb5daaecdf5cca1efb3c23290f18e3e1d2a64ff6f70c25118f8a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327050"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategoryCollectionPage categories = graphClient.education().classes("a17025d0-62a8-4450-9e6e-db31d8c8feb8").assignments("1fdf61ee-c129-4960-9b7c-8df159aa64b0").categories()
    .buildRequest()
    .get();

```
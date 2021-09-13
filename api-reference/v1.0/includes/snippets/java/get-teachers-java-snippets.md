---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 539b469380b9302e549f5a3778537dfeb04060646e460abfd5fad28a6a8fddbb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158127"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUserCollectionWithReferencesPage teachers = graphClient.education().classes("{class-id}").teachers()
    .buildRequest()
    .get();

```
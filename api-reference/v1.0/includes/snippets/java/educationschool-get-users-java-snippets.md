---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 780be761ccabd6102a0bc13aabbdf34702169119
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973651"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUserCollectionWithReferencesPage users = graphClient.education().schools("{school-id}").users()
    .buildRequest()
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe9e2ed5aa6c6be9bf4d28ec7bba37c0e343c5d7
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668683"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClassCollectionWithReferencesPage taughtClasses = graphClient.education().classes("{educationClassId}").members("{educationUserId}").taughtClasses()
    .buildRequest()
    .get();

```
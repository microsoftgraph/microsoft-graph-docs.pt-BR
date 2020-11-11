---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99d4b77020dab59d747581458bf2237b867b9fbc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983277"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationSchoolCollectionWithReferencesPage schools = graphClient.education().me().schools()
    .buildRequest()
    .get();

```
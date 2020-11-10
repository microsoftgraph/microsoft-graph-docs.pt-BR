---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 09be8a9da1065008ea0d0b94207d061bdcd83c1d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953945"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage transitiveMemberOf = graphClient.groups("{id}").transitiveMemberOf()
    .buildRequest()
    .get();

```
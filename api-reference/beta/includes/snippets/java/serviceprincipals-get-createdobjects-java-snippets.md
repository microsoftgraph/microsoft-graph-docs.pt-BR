---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0f2925efd9bbe8c0d0fbb3d012eedb5d588644d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870045"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage createdObjects = graphClient.servicePrincipals("{id}").createdObjects()
    .buildRequest()
    .get();

```
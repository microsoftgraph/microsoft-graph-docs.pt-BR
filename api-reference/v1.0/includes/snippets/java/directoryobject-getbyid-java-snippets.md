---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: abad93bddcbc9d8fa7826b394055e0d9a6dae337566ba26b05395ed114e77da0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156662"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> idsList = new LinkedList<String>();
idsList.add("84b80893874940a3-97b7-68513b600544");
idsList.add("5d6059b6368d-45f8-91e18e07d485f1d0");

LinkedList<String> typesList = new LinkedList<String>();
typesList.add("user");

graphClient.directoryObjects()
    .getByIds(DirectoryObjectGetByIdsParameterSet
        .newBuilder()
        .withIds(idsList)
        .withTypes(typesList)
        .build())
    .buildRequest()
    .post();

```
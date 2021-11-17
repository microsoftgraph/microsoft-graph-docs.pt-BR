---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd4ae83720a5c3c17ae6bb68991470b41cbcddefa9dfb2d756b5a8d48a0d9e35
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159881"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> idsList = new LinkedList<String>();
idsList.add("String");
idsList.add("String");
idsList.add("String");

String memberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice";

graphClient.admin().windows().updates().updatableAssets("{updatableAssetGroupId}")
    .removeMembersById(UpdatableAssetRemoveMembersByIdParameterSet
        .newBuilder()
        .withIds(idsList)
        .withMemberEntityType(memberEntityType)
        .build())
    .buildRequest()
    .post();

```
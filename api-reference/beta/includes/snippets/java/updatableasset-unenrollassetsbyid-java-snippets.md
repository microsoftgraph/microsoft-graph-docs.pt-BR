---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3c2cbd93b738d90936113fca6bb5d3f86ee85d9e1c8ce272b4ada99b25d0030
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329238"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdateCategory updateCategory = UpdateCategory.FEATURE;

String memberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice";

LinkedList<String> idsList = new LinkedList<String>();
idsList.add("String");
idsList.add("String");
idsList.add("String");

graphClient.admin().windows().updates().updatableAssets()
    .unenrollAssetsById(UpdatableAssetUnenrollAssetsByIdParameterSet
        .newBuilder()
        .withUpdateCategory(updateCategory)
        .withMemberEntityType(memberEntityType)
        .withIds(idsList)
        .build())
    .buildRequest()
    .post();

```
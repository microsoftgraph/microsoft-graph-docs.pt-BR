---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad6f3a1552c82584a4acab6d681bac5e7dfc4432aa7c6ef01ca92d5e71085886
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275434"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdateCategory updateCategory = UpdateCategory.FEATURE;

LinkedList<UpdatableAsset> assetsList = new LinkedList<UpdatableAsset>();
AzureADDevice assets = new AzureADDevice();
assets.id = "String (identifier)";

assetsList.add(assets);
UpdatableAssetCollectionResponse updatableAssetCollectionResponse = new UpdatableAssetCollectionResponse();
updatableAssetCollectionResponse.value = assetsList;
UpdatableAssetCollectionPage updatableAssetCollectionPage = new UpdatableAssetCollectionPage(updatableAssetCollectionResponse, null);

graphClient.admin().windows().updates().updatableAssets()
    .unenrollAssets(UpdatableAssetUnenrollAssetsParameterSet
        .newBuilder()
        .withUpdateCategory(updateCategory)
        .withAssets(assetsList)
        .build())
    .buildRequest()
    .post();

```
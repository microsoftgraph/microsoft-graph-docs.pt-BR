---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c92c1aaf66185f78443da45421eed9f4610c2ed0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334153"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<UpdatableAsset> addMembersList = new LinkedList<UpdatableAsset>();
AzureADDevice addMembers = new AzureADDevice();
addMembers.id = "String (identifier)";

addMembersList.add(addMembers);
UpdatableAssetCollectionResponse updatableAssetCollectionResponse = new UpdatableAssetCollectionResponse();
updatableAssetCollectionResponse.value = addMembersList;
UpdatableAssetCollectionPage updatableAssetCollectionPage = new UpdatableAssetCollectionPage(updatableAssetCollectionResponse, null);

LinkedList<UpdatableAsset> removeMembersList = new LinkedList<UpdatableAsset>();
AzureADDevice removeMembers = new AzureADDevice();
removeMembers.id = "String (identifier)";

removeMembersList.add(removeMembers);
UpdatableAssetCollectionResponse updatableAssetCollectionResponse = new UpdatableAssetCollectionResponse();
updatableAssetCollectionResponse.value = removeMembersList;
UpdatableAssetCollectionPage updatableAssetCollectionPage = new UpdatableAssetCollectionPage(updatableAssetCollectionResponse, null);

LinkedList<UpdatableAsset> addExclusionsList = new LinkedList<UpdatableAsset>();
AzureADDevice addExclusions = new AzureADDevice();
addExclusions.id = "String (identifier)";

addExclusionsList.add(addExclusions);
UpdatableAssetCollectionResponse updatableAssetCollectionResponse = new UpdatableAssetCollectionResponse();
updatableAssetCollectionResponse.value = addExclusionsList;
UpdatableAssetCollectionPage updatableAssetCollectionPage = new UpdatableAssetCollectionPage(updatableAssetCollectionResponse, null);

LinkedList<UpdatableAsset> removeExclusionsList = new LinkedList<UpdatableAsset>();
AzureADDevice removeExclusions = new AzureADDevice();
removeExclusions.id = "String (identifier)";

removeExclusionsList.add(removeExclusions);
UpdatableAssetCollectionResponse updatableAssetCollectionResponse = new UpdatableAssetCollectionResponse();
updatableAssetCollectionResponse.value = removeExclusionsList;
UpdatableAssetCollectionPage updatableAssetCollectionPage = new UpdatableAssetCollectionPage(updatableAssetCollectionResponse, null);

graphClient.admin().windows().updates().deployments("{deploymentId}").audience()
    .updateAudience(DeploymentAudienceUpdateAudienceParameterSet
        .newBuilder()
        .withAddMembers(addMembersList)
        .withRemoveMembers(removeMembersList)
        .withAddExclusions(addExclusionsList)
        .withRemoveExclusions(removeExclusionsList)
        .build())
    .buildRequest()
    .post();

```
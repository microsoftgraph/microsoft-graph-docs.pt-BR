---
title: Tipo de recurso mobileAppRelationshipState
description: Descreve os detalhes de status de instalação do aplicativo filho no contexto de UPN e id do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 58927afdfce4336eb3d0abfcf234f9c1dc1fe77e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803038"
---
# <a name="mobileapprelationshipstate-resource-type"></a>Tipo de recurso mobileAppRelationshipState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve os detalhes de status de instalação do aplicativo filho no contexto de UPN e id do dispositivo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|sourceIds|Coleção de cadeias de caracteres|A coleção de IDs do aplicativo móvel de origem.|
|targetId|Cadeia de caracteres|A ID do aplicativo de destino relacionado.|
|targetDisplayName|Cadeia de caracteres|O nome de exibição do aplicativo de destino relacionado.|
|deviceId|Cadeia de caracteres|A ID do dispositivo correspondente.|
|installState|[resultantAppState](../resources/intune-apps-resultantappstate.md)|O estado de instalação do aplicativo de destino. Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|O detalhe de estado de instalação do aplicativo. Os valores possíveis são: `noAdditionalDetails` , `dependencyFailedToInstall` , , `dependencyWithRequirementsNotMet` `dependencyPendingReboot` , `dependencyWithAutoInstallDisabled` `supersededAppUninstallFailed` `supersededAppUninstallPendingReboot` `removingSupersededApps` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `uninstallPendingReboot` `supersedingAppsDetected` `supersededAppsDetected` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` `untargetedSupersedingAppsDetected` `appRemovedBySupersedence` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `contentDownloaded` `supersedingAppsNotApplicable` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` .|
|errorCode|Int32|O código de erro para instalar ou desinstalar falhas do aplicativo de destino.|
|targetLastSyncDateTime|DateTimeOffset|O último tempo de sincronização do aplicativo de destino.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppRelationshipState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationshipState",
  "sourceIds": [
    "String"
  ],
  "targetId": "String",
  "targetDisplayName": "String",
  "deviceId": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "targetLastSyncDateTime": "String (timestamp)"
}
```




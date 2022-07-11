---
title: Tipo de recurso mobileAppInstallStatus
description: Contém propriedades para o estado de instalação de um aplicativo móvel para um dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: efcf9d78aecd7ba49e5630473e790d3ed7c37406
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671229"
---
# <a name="mobileappinstallstatus-resource-type"></a>Tipo de recurso mobileAppInstallStatus

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o estado de instalação de um aplicativo móvel para um dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppInstallStatuses](../api/intune-apps-mobileappinstallstatus-list.md)|[Coleção mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Listar propriedades e relações dos objetos [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|
|[Obter mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Ler propriedades e relações do objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|
|[Criar mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-create.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Crie um novo [objeto mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|
|[Excluir mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-delete.md)|Nenhum|Exclui um [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).|
|[Atualizar mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-update.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Atualize as propriedades de um [objeto mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|deviceName|String|Nome do dispositivo|
|deviceId|Cadeia de caracteres|ID do Dispositivo|
|lastSyncDateTime|DateTimeOffset|Hora da última sincronização|
|mobileAppInstallStatusValue|[resultantAppState](../resources/intune-apps-resultantappstate.md)|O estado de instalação do aplicativo. Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installState|[resultantAppState](../resources/intune-apps-resultantappstate.md)|O estado de instalação do aplicativo. Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|Os detalhes do estado de instalação do aplicativo. Os valores possíveis são: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `supersededAppUninstallFailed`, , `vppAppHasUpdateAvailable``supersededAppUninstallPendingReboot``processorArchitectureNotApplicable``supersedingAppsDetected``minimumDiskSpaceNotMet``uninstallPendingReboot``minimumOsVersionNotMet``supersededAppsDetected``userRejectedUpdate``supersedingAppsNotApplicable``seeInstallErrorCode``powerShellScriptRequirementNotMet``autoInstallDisabled``registryRequirementNotMet``minimumLogicalProcessorCountNotMet``contentDownloaded``minimumPhysicalMemoryNotMet``minimumCpuSpeedNotMet``platformNotApplicable``fileSystemRequirementNotMet``installingDependencies``pendingReboot``seeUninstallErrorCode``appRemovedBySupersedence``userIsNotLoggedIntoAppStore``managedAppNoLongerPresent``untargetedSupersedingAppsDetected``removingSupersededApps``iosAppStoreUpdateFailedToInstall``userRejectedInstall`.|
|errorCode|Int32|O código de erro para falhas de instalação ou desinstalação.|
|osVersion|String|Versão do SO|
|osDescription|Cadeia de caracteres|Descrição do sistema operacional|
|userName|Cadeia de caracteres|Nome de Usuário do Dispositivo|
|userPrincipalName|Cadeia de caracteres|Nome UPN|
|displayVersion|Cadeia de Caracteres|Versão legível humana do aplicativo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|aplicativo|[mobileApp](../resources/intune-apps-mobileapp.md)|O link de navegação para o aplicativo móvel.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "mobileAppInstallStatusValue": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "displayVersion": "String"
}
```





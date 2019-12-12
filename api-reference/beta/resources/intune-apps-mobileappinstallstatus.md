---
title: tipo de recurso mobileAppInstallStatus
description: Contém propriedades para o estado de instalação de um aplicativo móvel para um dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 95d6d694da12fe4615ada0d0a2a19f5d7d992980
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955614"
---
# <a name="mobileappinstallstatus-resource-type"></a>tipo de recurso mobileAppInstallStatus

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o estado de instalação de um aplicativo móvel para um dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppInstallStatuses](../api/intune-apps-mobileappinstallstatus-list.md)|coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Listar Propriedades e relações dos objetos [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|
|[Obter mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Leia as propriedades e as relações do objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|
|[Criar mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-create.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Criar um novo objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|
|[Excluir mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-delete.md)|Nenhum|Exclui [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).|
|[Atualizar mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-update.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Atualiza as propriedades de um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|deviceName|Cadeia de Caracteres|Nome do dispositivo|
|deviceId|Cadeia de Caracteres|ID do dispositivo|
|lastSyncDateTime|DateTimeOffset|Hora da data da última sincronização|
|mobileAppInstallStatusValue|[resultantAppState](../resources/intune-shared-resultantappstate.md)|O estado de instalação do aplicativo. Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installState|[resultantAppState](../resources/intune-shared-resultantappstate.md)|O estado de instalação do aplicativo. Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|Os detalhes do estado de instalação do aplicativo. Os valores possíveis são: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.|
|errorCode|Int32|O código de erro para instalação ou desinstalação de falhas.|
|osVersion|String|Versão do sistema operacional|
|osDescription|Cadeia de Caracteres|Descrição do sistema operacional|
|userName|Cadeia de caracteres|Nome de usuário do dispositivo|
|userPrincipalName|String|Nome UPN|
|displayVersion|Cadeia de Caracteres|Versão de leitura humana do aplicativo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|aplicativo|[mobileApp](../resources/intune-shared-mobileapp.md)|O link de navegação para o aplicativo móvel.|

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




---
title: Tipo de recurso androidForWorkSettings
description: Configurações para o Android for Work.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49e8f0efc187653b6070296ff8c9ed43967056b1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780711"
---
# <a name="androidforworksettings-resource-type"></a>Tipo de recurso androidForWorkSettings

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configurações para o Android for Work.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Get androidForWorkSettings](../api/intune-androidforwork-androidforworksettings-get.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Ler propriedades e relações do objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).|
|[Atualizar androidForWorkSettings](../api/intune-androidforwork-androidforworksettings-update.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Atualizar as propriedades de um objeto de [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).|
|[Ação requestSignupUrl](../api/intune-androidforwork-androidforworksettings-requestsignupurl.md)|String|Ainda não documentado|
|[Ação completeSignup](../api/intune-androidforwork-androidforworksettings-completesignup.md)|Nenhuma|Ainda não documentado|
|[Ação syncApps](../api/intune-androidforwork-androidforworksettings-syncapps.md)|Nenhuma|Ainda não documentado|
|[ação unbind](../api/intune-androidforwork-androidforworksettings-unbind.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador de configurações do Android for Work|
|bindStatus|[androidForWorkBindStatus](../resources/intune-androidforwork-androidforworkbindstatus.md)|Vincule o status do locatário à API do Google EMM. Os valores possíveis são: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Hora da conclusão da última sincronização do aplicativo|
|lastAppSyncStatus|[androidForWorkSyncStatus](../resources/intune-androidforwork-androidforworksyncstatus.md)|Resultado da última sincronização do aplicativo. Os valores possíveis são: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|Cadeia de caracteres|UPN proprietária que criou a empresa|
|ownerOrganizationName|String|Nome da organização usada ao integrar o Android for Work|
|lastModifiedDateTime|DateTimeOffset|Hora da última modificação das configurações do Android for Work|
|enrollmentTarget|[androidForWorkEnrollmentTarget](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|Indica quais usuários podem registrar dispositivos no Android para gerenciamento de dispositivos de trabalho. Os valores possíveis são: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|String collection|Especifica a quais grupos AAD podem registrar dispositivos no gerenciamento de dispositivos do Android for Work se enrollmentTarget estiver definido como 'Direcionado'|
|deviceOwnerManagementEnabled|Booliano|Indica se esta conta está comprovando o gerenciamento de proprietário do dispositivo Android com o CloudDPC.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ],
  "deviceOwnerManagementEnabled": true
}
```






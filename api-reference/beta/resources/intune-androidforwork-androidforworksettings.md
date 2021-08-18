---
title: Tipo de recurso androidForWorkSettings
description: Configurações para o Android for Work.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b696638dbf3c7cdc00b1d47de782de53f92949078dc31d50d96decca9f6d236b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54233074"
---
# <a name="androidforworksettings-resource-type"></a>Tipo de recurso androidForWorkSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configurações para o Android for Work.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter androidForWorkSettings](../api/intune-androidforwork-androidforworksettings-get.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Ler propriedades e relações de objetos de [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).|
|[Atualizar androidForWorkSettings](../api/intune-androidforwork-androidforworksettings-update.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Atualizar as propriedades de um objeto de [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).|
|[Ação requestSignupUrl](../api/intune-androidforwork-androidforworksettings-requestsignupurl.md)|Cadeia de caracteres|Ainda não documentado|
|[Ação completeSignup](../api/intune-androidforwork-androidforworksettings-completesignup.md)|Nenhum|Ainda não documentado|
|[Ação syncApps](../api/intune-androidforwork-androidforworksettings-syncapps.md)|Nenhum|Ainda não documentado|
|[Ação de desvincular](../api/intune-androidforwork-androidforworksettings-unbind.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de configurações do Android for Work|
|bindStatus|[androidForWorkBindStatus](../resources/intune-androidforwork-androidforworkbindstatus.md)|Vincular o status do locatário à API de EMM do Google. Os valores possíveis são: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Hora da conclusão da última sincronização do aplicativo|
|lastAppSyncStatus|[androidForWorkSyncStatus](../resources/intune-androidforwork-androidforworksyncstatus.md)|Último resultado de sincronização de aplicativo. Os possíveis valores são: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|String|UPN proprietária que criou a empresa|
|ownerOrganizationName|String|Nome da organização usada ao integrar o Android for Work|
|lastModifiedDateTime|DateTimeOffset|Hora da última modificação das configurações do Android for Work|
|enrollmentTarget|[androidForWorkEnrollmentTarget](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|Indica quais usuários podem registrar dispositivos no gerenciamento de dispositivos Android for Work. Os valores possíveis são: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|String collection|Especifica a quais grupos AAD podem registrar dispositivos no gerenciamento de dispositivos do Android for Work se enrollmentTarget estiver definido como 'Direcionado'|
|deviceOwnerManagementEnabled|Boolean|Indica se essa conta está sendo reativada para o Gerenciamento de Proprietários de Dispositivos Android com o CloudDPC.|

## <a name="relationships"></a>Relações
Nenhum

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





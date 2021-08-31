---
title: Tipo de recurso deviceManagementIntent
description: Entidade que representa a intenção de aplicar configurações a um dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 465abb5a003817f596eb70067b8ac6b5a28e94e7
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58759432"
---
# <a name="devicemanagementintent-resource-type"></a>Tipo de recurso deviceManagementIntent

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa a intenção de aplicar configurações a um dispositivo

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementIntents](../api/intune-deviceintent-devicemanagementintent-list.md)|[Coleção deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Listar propriedades e relações dos [objetos deviceManagementIntent.](../resources/intune-deviceintent-devicemanagementintent.md)|
|[Obter deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-get.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Leia propriedades e relações do [objeto deviceManagementIntent.](../resources/intune-deviceintent-devicemanagementintent.md)|
|[Criar deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-create.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Crie um novo [objeto deviceManagementIntent.](../resources/intune-deviceintent-devicemanagementintent.md)|
|[Excluir deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-delete.md)|Nenhum(a)|Exclui um [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md).|
|[Atualizar deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-update.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Atualize as propriedades de [um objeto deviceManagementIntent.](../resources/intune-deviceintent-devicemanagementintent.md)|
|[ação updateSettings](../api/intune-deviceintent-devicemanagementintent-updatesettings.md)|Nenhuma|Ainda não documentado|
|[Ação migrateToTemplate](../api/intune-deviceintent-devicemanagementintent-migratetotemplate.md)|Nenhuma|Ainda não documentado|
|[Ação createCopy](../api/intune-deviceintent-devicemanagementintent-createcopy.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Ainda não documentado|
|[atribuir ação](../api/intune-deviceintent-devicemanagementintent-assign.md)|Nenhuma|Ainda não documentado|
|[função compare](../api/intune-deviceintent-devicemanagementintent-compare.md)|[Coleção deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID de intenção|
|displayName|Cadeia de caracteres|O nome de exibição dado pelo usuário|
|descrição|Cadeia de caracteres|A descrição dada pelo usuário|
|isAssigned|Boolean|Significa se a intenção é atribuída ou não aos usuários|
|lastModifiedDateTime|DateTimeOffset|Quando a intenção foi modificada pela última vez|
|templateId|Cadeia de caracteres|A ID do modelo de que essa intenção foi criada (se alguma)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância entity.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|settings|[Coleção deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Coleção de todas as configurações a serem aplicadas|
|categories|[Coleção deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Coleção de categorias de configuração dentro da intenção|
|assignments|[Coleção deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Coleção de atribuições|
|deviceSettingStateSummaries|[coleção deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Coleção de configurações e seus estados e contagens de dispositivos que pertencem ao estado correspondente para todas as configurações dentro da intenção|
|deviceStates|[Coleção deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Coleção de estados de todos os dispositivos aos que a intenção é aplicada|
|userStates|[Coleção deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Coleção de estados de todos os usuários aos que a intenção é aplicada|
|deviceStateSummary|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|Um resumo dos estados do dispositivo e das contagens de dispositivos que pertencem ao estado correspondente para todos os dispositivos aos que a intenção é aplicada|
|userStateSummary|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|Um resumo dos estados do usuário e contagens de usuários que pertencem ao estado correspondente para todos os usuários aos que a intenção é aplicada|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isAssigned": true,
  "lastModifiedDateTime": "String (timestamp)",
  "templateId": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```




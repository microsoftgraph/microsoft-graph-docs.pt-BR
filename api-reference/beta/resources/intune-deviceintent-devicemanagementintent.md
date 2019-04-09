---
title: tipo de recurso deviceManagementIntent
description: Entidade que representa uma intenção de aplicar configurações a um dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 909b071279b35c2ffec4c27b3431d25f7da8ac46
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524243"
---
# <a name="devicemanagementintent-resource-type"></a>tipo de recurso deviceManagementIntent

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa uma intenção de aplicar configurações a um dispositivo

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementIntents](../api/intune-deviceintent-devicemanagementintent-list.md)|coleção [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Listar Propriedades e relações dos objetos [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) .|
|[Obter deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-get.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Leia as propriedades e as relações do objeto [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) .|
|[Criar deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-create.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Criar um novo objeto [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) .|
|[Excluir deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-delete.md)|Nenhum|Exclui [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md).|
|[Atualizar deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-update.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Atualiza as propriedades de um objeto [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) .|
|[ação updateSettings](../api/intune-deviceintent-devicemanagementintent-updatesettings.md)|Nenhuma|Ainda não documentado|
|[atribuir ação](../api/intune-deviceintent-devicemanagementintent-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID de intenção|
|displayName|Cadeia de Caracteres|O nome de exibição fornecido pelo usuário|
|description|String|Descrição fornecida pelo usuário|
|isAssigned|Boolean|Significa se a intenção é atribuída ou não aos usuários|
|lastModifiedDateTime|DateTimeOffset|Quando a intenção foi modificada pela última vez|
|templateId|Cadeia de Caracteres|A ID do modelo de que esta intenção foi criada (se houver)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|settings|coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Coleção de todas as configurações a serem aplicadas|
|Categorias|coleção [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Conjunto de categorias de configuração dentro da intenção|
|assignments|coleção [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Coleção de atribuições|
|deviceSettingStateSummaries|coleção [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Conjunto de configurações e seus Estados e contagens de dispositivos que pertencem ao estado correspondente de todas as configurações dentro da intenção|
|deviceStates|coleção [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Conjunto de Estados de todos os dispositivos aos quais a intenção é aplicada|
|userStates|coleção [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|Conjunto de Estados de todos os usuários aos quais a intenção é aplicada|
|deviceStateSummary|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|Um resumo dos Estados do dispositivo e as contagens de dispositivos que pertencem ao estado correspondente de todos os dispositivos aos quais a intenção é aplicada|
|userStateSummary|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|Um resumo dos Estados do usuário e as contagens de usuários que pertencem ao estado correspondente de todos os usuários aos quais a intenção é aplicada|

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
  "templateId": "String"
}
```








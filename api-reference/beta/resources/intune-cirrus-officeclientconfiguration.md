---
title: tipo de recurso Conjuntoofficeclientconfiguration
description: Configuração de cliente do Office.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3688503cf19d8cebe51b4afe7abd1563257f9192
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004756"
---
# <a name="officeclientconfiguration-resource-type"></a>tipo de recurso Conjuntoofficeclientconfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração de cliente do Office.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar officeClientConfigurations](../api/intune-cirrus-officeclientconfiguration-list.md)|coleção [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|Listar Propriedades e relações dos objetos [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .|
|[Obter Conjuntoofficeclientconfiguration](../api/intune-cirrus-officeclientconfiguration-get.md)|[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|Leia as propriedades e as relações do objeto [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .|
|[atribuir ação](../api/intune-cirrus-officeclientconfiguration-assign.md)|coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Substituir todos os grupos de destino de uma política.|
|[ação updatePriorities](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|Nenhum|Atualizar prioridades de política.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID da política de configuração de cliente do Office.|
|userPreferencePayload|Fluxo|Cadeia de caracteres JSON das configurações de preferência no formato binário, esses valores podem ser substituídos pelo usuário.|
|policyPayload|Fluxo|Cadeia de caracteres JSON de configurações de política no formato binário, esses valores não podem ser alterados pelo usuário.|
|descrição|String|Ainda não documentado|
|displayName|String|Descrição fornecida pelo administrador da política de configuração de cliente do Office.|
|lastModifiedDateTime|DateTime|Carimbo de data/hora da última modificação da política.|
|prioridade|Int32|O valor de prioridade deve ser um valor exclusivo para cada política em um locatário e será usado para resolução de conflitos, a prioridade média de valores menores é alta.|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Resumo de check-in do usuário da política.|
|checkinStatuses|coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)|Lista de status de check-in do cliente do Office.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|A lista de atribuições de grupo para a política.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfiguration",
  "id": "String (identifier)",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "String",
  "displayName": "String",
  "priority": 1024,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ]
}
```




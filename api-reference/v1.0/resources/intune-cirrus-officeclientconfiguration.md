---
title: Tipo de recurso officeClientConfiguration
description: Office Configuração do Cliente.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 181e06de36176c5d2dbbdb8d1794ae64390ee71b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752839"
---
# <a name="officeclientconfiguration-resource-type"></a>Tipo de recurso officeClientConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Office Configuração do Cliente.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar officeClientConfigurations](../api/intune-cirrus-officeclientconfiguration-list.md)|[Coleção officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|Listar propriedades e relações dos [objetos officeClientConfiguration.](../resources/intune-cirrus-officeclientconfiguration.md)|
|[Obter officeClientConfiguration](../api/intune-cirrus-officeclientconfiguration-get.md)|[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|Leia propriedades e relações do [objeto officeClientConfiguration.](../resources/intune-cirrus-officeclientconfiguration.md)|
|[atribuir ação](../api/intune-cirrus-officeclientconfiguration-assign.md)|[Coleção officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Substitua todos os grupos direcionados por uma política.|
|[ação updatePriorities](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|Nenhum|Atualizar prioridades de política.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID da política de configuração do cliente do office.|
|userPreferencePayload|Stream|Configurações de preferência Cadeia de caracteres JSON no formato binário, esses valores podem ser substituídos pelo usuário.|
|policyPayload|Stream|Configurações de política Cadeia de caracteres JSON em formato binário, esses valores não podem ser alterados pelo usuário.|
|description|String|Ainda não documentado|
|displayName|String|O administrador forneceu a descrição da política de configuração do cliente do office.|
|lastModifiedDateTime|DateTime|Carimbo de data da última modificação da política.|
|prioridade|Int32|O valor de prioridade deve ser o valor exclusivo para cada política em um locatário e será usado para resolução de conflitos, valores mais baixos a prioridade média é alta.|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Resumo de check-in do usuário para a política.|
|checkinStatuses|[Coleção officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)|Lista de status de check-in do cliente do office.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|A lista de atribuições de grupo para a política.|

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





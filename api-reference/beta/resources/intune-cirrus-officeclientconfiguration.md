---
title: tipo de recurso de officeClientConfiguration
description: Configuração do cliente do Office.
author: tfitzmac
ms.openlocfilehash: 67a7845a2e0327e2e5de37d424274f6e2ee35604
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303833"
---
# <a name="officeclientconfiguration-resource-type"></a>tipo de recurso de officeClientConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configuração do cliente do Office.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista officeClientConfigurations](../api/intune-cirrus-officeclientconfiguration-list.md)|coleção [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|Lista as propriedades e os relacionamentos dos objetos [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .|
|[Obter officeClientConfiguration](../api/intune-cirrus-officeclientconfiguration-get.md)|[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|Leia as propriedades e os relacionamentos do objeto [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .|
|[Ação assign](../api/intune-cirrus-officeclientconfiguration-assign.md)|coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Substitua direcionados todos os grupos de uma política.|
|[ação de updatePriorities](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|Nenhum|Atualize as prioridades de política.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID da diretiva de configuração do cliente do office.|
|userPreferencePayload|Stream|Configurações de preferência JSON da cadeia de caracteres em formato binário, esses valores podem ser substituídos pelo usuário.|
|policyPayload|Stream|Configurações de diretiva JSON da cadeia de caracteres em formato binário, esses valores não podem ser alterados pelo usuário.|
|description|String|Ainda não documentado|
|displayName|String|Admin fornecida a descrição do cliente do office política de configuração.|
|lastModifiedDateTime|DateTime|Carimbo de data e hora modificadas por último da política.|
|prioridade|Int32|Valor de prioridade deve ser um valor exclusivo para cada política em um locatário e será usado para resolução de conflito, valores inferiores média de prioridade é alta.|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Check-in do resumo do usuário para a política.|
|checkinStatuses|coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)|Lista de status de check-in do cliente do office.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|A lista de atribuições para a política de grupo.|

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




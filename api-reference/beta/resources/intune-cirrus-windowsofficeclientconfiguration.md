---
title: tipo de recurso windowsOfficeClientConfiguration
description: Entidade que descreve as configurações de política do Office para Windows.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 05e52f7f7fbef4748259bde1f048203f4b49a32e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004782"
---
# <a name="windowsofficeclientconfiguration-resource-type"></a>tipo de recurso windowsOfficeClientConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que descreve as configurações de política do Office para Windows.

Herda de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsOfficeClientConfigurations](../api/intune-cirrus-windowsofficeclientconfiguration-list.md)|coleção [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|Listar Propriedades e relações dos objetos [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .|
|[Obter windowsOfficeClientConfiguration](../api/intune-cirrus-windowsofficeclientconfiguration-get.md)|[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|Leia as propriedades e as relações do objeto [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .|
|[Criar windowsOfficeClientConfiguration](../api/intune-cirrus-windowsofficeclientconfiguration-create.md)|[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|Criar um novo objeto [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .|
|[Excluir windowsOfficeClientConfiguration](../api/intune-cirrus-windowsofficeclientconfiguration-delete.md)|Nenhum|Exclui [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).|
|[Atualizar windowsOfficeClientConfiguration](../api/intune-cirrus-windowsofficeclientconfiguration-update.md)|[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|Atualiza as propriedades de um objeto [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID da política de configuração de cliente do Office. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userPreferencePayload|Fluxo|Cadeia de caracteres JSON das configurações de preferência no formato binário, esses valores podem ser substituídos pelo usuário. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|policyPayload|Fluxo|Cadeia de caracteres JSON de configurações de política no formato binário, esses valores não podem ser alterados pelo usuário. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|descrição|String|Descrição fornecida pelo administrador da política de configuração de cliente do Office. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|displayName|String|Nome fornecido pelo administrador da política de configuração de cliente do Office. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|prioridade|Int32|O valor de prioridade deve ser um valor exclusivo para cada política em um locatário e será usado para resolução de conflitos, a prioridade média de valores menores é alta. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|lastModifiedDateTime|DateTime|Carimbo de data/hora da última modificação da política. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Resumo de check-in do usuário da política. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|checkinStatuses|coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)|Lista de status de check-in do cliente do Office. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|A lista de atribuições de grupo para a política. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsOfficeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
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




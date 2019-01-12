---
title: tipo de recurso de windowsOfficeClientSecurityConfiguration
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0ebb53188e0542e33735b632a7eb2adbbaaea8a3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927335"
---
# <a name="windowsofficeclientsecurityconfiguration-resource-type"></a>tipo de recurso de windowsOfficeClientSecurityConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ainda não documentado

Herda de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista windowsOfficeClientSecurityConfigurations](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-list.md)|coleção [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|Lista as propriedades e os relacionamentos dos objetos [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .|
|[Obter windowsOfficeClientSecurityConfiguration](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-get.md)|[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|Leia as propriedades e os relacionamentos do objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .|
|[Criar windowsOfficeClientSecurityConfiguration](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-create.md)|[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|Crie um novo objeto de [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .|
|[Excluir windowsOfficeClientSecurityConfiguration](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-delete.md)|Nenhum|Exclui um [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).|
|[Atualizar windowsOfficeClientSecurityConfiguration](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-update.md)|[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|Atualize as propriedades de um objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID da diretiva de configuração do cliente do office. Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userPreferencePayload|Stream|Configurações de preferência JSON da cadeia de caracteres em formato binário, esses valores podem ser substituídos pelo usuário. Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|policyPayload|Stream|Configurações de diretiva JSON da cadeia de caracteres em formato binário, esses valores não podem ser alterados pelo usuário. Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|description|Cadeia de caracteres|Admin fornecida a descrição do cliente do office política de configuração. Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|displayName|Cadeia de caracteres|Admin fornecido o nome da política de configuração do cliente office. Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|prioridade|Int32|Valor de prioridade deve ser um valor exclusivo para cada política em um locatário e será usado para resolução de conflito, valores inferiores média de prioridade é alta. Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|lastModifiedDateTime|DateTime|Carimbo de data e hora modificadas por último da política. Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Check-in do resumo do usuário para a política. Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|checkinStatuses|coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)|Lista de status de check-in do cliente do office. Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|A lista de atribuições para a política de grupo. Herdado de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsOfficeClientSecurityConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
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




---
title: Tipo de recurso windowsOfficeClientSecurityConfiguration
description: Ainda não documentado
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2a658405e3520c468c30413cbc628416a8551513
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101846"
---
# <a name="windowsofficeclientsecurityconfiguration-resource-type"></a>Tipo de recurso windowsOfficeClientSecurityConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

Herda de [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsOfficeClientSecurityConfigurations](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-list.md)|[Coleção windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|Listar propriedades e relações dos [objetos windowsOfficeClientSecurityConfiguration.](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|
|[Obter windowsOfficeClientSecurityConfiguration](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-get.md)|[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|Leia propriedades e relações do [objeto windowsOfficeClientSecurityConfiguration.](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|
|[Criar windowsOfficeClientSecurityConfiguration](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-create.md)|[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|Crie um novo [objeto windowsOfficeClientSecurityConfiguration.](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|
|[Excluir windowsOfficeClientSecurityConfiguration](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-delete.md)|Nenhum|Exclui um [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).|
|[Atualizar windowsOfficeClientSecurityConfiguration](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-update.md)|[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|Atualize as propriedades de um [objeto windowsOfficeClientSecurityConfiguration.](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID da política de configuração do cliente do office. Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userPreferencePayload|Stream|Configurações de preferência Cadeia de caracteres JSON no formato binário, esses valores podem ser substituídos pelo usuário. Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|policyPayload|Stream|Configurações de política Cadeia de caracteres JSON em formato binário, esses valores não podem ser alterados pelo usuário. Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da política de configuração do cliente do office. Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da política de configuração do cliente do office. Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|prioridade|Int32|O valor de prioridade deve ser o valor exclusivo para cada política em um locatário e será usado para resolução de conflitos, valores mais baixos a prioridade média é alta. Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|lastModifiedDateTime|DateTime|Carimbo de data da última modificação da política. Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Resumo de check-in do usuário para a política. Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|checkinStatuses|[Coleção officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)|Lista de status de check-in do cliente do office. Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|A lista de atribuições de grupo para a política. Herdado [do officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|

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




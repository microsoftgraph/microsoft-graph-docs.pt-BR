---
title: Criar windowsOfficeClientSecurityConfiguration
description: Criar um novo objeto windowsOfficeClientSecurityConfiguration.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aea9c8207d904eb001b0c3bf86a42233385fd2ea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958778"
---
# <a name="create-windowsofficeclientsecurityconfiguration"></a>Criar windowsOfficeClientSecurityConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID da política de configuração de cliente do Office. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userPreferencePayload|Fluxo|Cadeia de caracteres JSON das configurações de preferência no formato binário, esses valores podem ser substituídos pelo usuário. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|policyPayload|Fluxo|Cadeia de caracteres JSON de configurações de política no formato binário, esses valores não podem ser alterados pelo usuário. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|descrição|String|Descrição fornecida pelo administrador da política de configuração de cliente do Office. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|displayName|String|Nome fornecido pelo administrador da política de configuração de cliente do Office. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|assignments|coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|A lista de atribuições de grupo para a política.. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|prioridade|Int32|O valor de prioridade deve ser um valor exclusivo para cada política em um locatário e será usado para resolução de conflitos, a prioridade média de valores menores é alta. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|lastModifiedDateTime|DateTime|Carimbo de data/hora da última modificação da política. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Resumo de check-in do usuário da política. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|checkinStatuses|coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)|Lista de status de check-in do cliente do Office. Herdado de [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|




## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
Content-type: application/json
Content-length: 1028

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1077

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
  "id": "f90ca1a5-a1a5-f90c-a5a1-0cf9a5a10cf9",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```




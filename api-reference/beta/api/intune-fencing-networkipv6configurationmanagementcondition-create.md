---
title: Criar networkIPv6ConfigurationManagementCondition
description: Criar um novo objeto networkIPv6ConfigurationManagementCondition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d7ad4e3796794456141fc3f1f0f90667f228be58
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804685"
---
# <a name="create-networkipv6configurationmanagementcondition"></a>Criar networkIPv6ConfigurationManagementCondition

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto networkIPv6ConfigurationManagementCondition.

A tabela a seguir mostra as propriedades que são necessárias ao criar networkIPv6ConfigurationManagementCondition.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da condição de gerenciamento. Valor gerado pelo sistema atribuído quando criado. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|String|Nome exclusivo para a condição de gerenciamento. Usado em expressões de condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|Cadeia de caracteres|O nome do administrador definido da condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|Cadeia de caracteres|A descrição definida pelo administrador da condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|A hora em que a condição de gerenciamento foi criada. Lado do serviço gerado. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|A hora em que a condição de gerenciamento foi modificada pela última vez. Atualizado o lado do serviço. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag da condição de gerenciamento. Atualizado o lado do serviço. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|As plataformas aplicáveis para essa condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md). Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|ipV6Prefix|String|A sub-rede IPv6 a ser conectada. por exemplo, 2001: DB8::/32|
|ipV6Gateway|String|O endereço do gateway IPv6 para. por exemplo, 2001: DB8:: 1|
|ipV6DNSServerList|Coleção de cadeias de caracteres|Servidores DNS IPv6 configurados para o adaptador.|
|dnsSuffixList|Coleção de cadeias de caracteres|Sufixos DNS válidos para a rede atual. por exemplo, seattle.contoso.com|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "25811206-1206-2581-0612-812506128125",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```





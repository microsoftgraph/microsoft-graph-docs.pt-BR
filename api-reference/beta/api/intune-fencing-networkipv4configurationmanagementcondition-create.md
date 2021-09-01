---
title: Criar networkIPv4ConfigurationManagementCondition
description: Crie um novo objeto networkIPv4ConfigurationManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88d9e380f5abe42feac71488f53fb14d06936f9d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820243"
---
# <a name="create-networkipv4configurationmanagementcondition"></a>Criar networkIPv4ConfigurationManagementCondition

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto networkIPv4ConfigurationManagementCondition.](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

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
No corpo da solicitação, fornece uma representação JSON para o objeto networkIPv4ConfigurationManagementCondition.

A tabela a seguir mostra as propriedades que são necessárias ao criar networkIPv4ConfigurationManagementCondition.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da condição de gerenciamento. Valor gerado pelo sistema atribuído quando criado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|Nome único|Cadeia de caracteres|Nome exclusivo para a condição de gerenciamento. Usado em expressões de condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|O nome definido pelo administrador da condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|String|A descrição definida pelo administrador da condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|A hora em que a condição de gerenciamento foi criada. Lado de serviço gerado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|O tempo em que a condição de gerenciamento foi modificada pela última vez. Lado do serviço atualizado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag da condição de gerenciamento. Lado do serviço atualizado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[Coleção devicePlatformType](../resources/intune-fencing-deviceplatformtype.md)|As plataformas aplicáveis para essa condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md). Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|ipV4Prefix|String|A sub-rede IPv4 a ser conectada. por exemplo, 10.0.0.0/8|
|ipV4Gateway|Cadeia de caracteres|O endereço de gateway IPv4. por exemplo, 10.0.0.0|
|ipV4DHCPServer|Cadeia de caracteres|O endereço IPv4 do servidor DHCP para o adaptador.|
|ipV4DNSServerList|Coleção de cadeias de caracteres|Os servidores DNS IPv4 configurados para o adaptador.|
|dnsSuffixList|Coleção String|Sufixos DNS válidos para a rede atual. por exemplo, seattle.contoso.com|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 529

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
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
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```




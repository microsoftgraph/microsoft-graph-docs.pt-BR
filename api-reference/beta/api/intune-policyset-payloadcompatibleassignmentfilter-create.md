---
title: Criar payloadCompatibleAssignmentFilter
description: Crie um novo objeto payloadCompatibleAssignmentFilter.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d105574eb8b901eead86ba9329a02c18b16fc599
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60492507"
---
# <a name="create-payloadcompatibleassignmentfilter"></a>Criar payloadCompatibleAssignmentFilter

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto payloadCompatibleAssignmentFilter.](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/assignmentFilters
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto payloadCompatibleAssignmentFilter.

A tabela a seguir mostra as propriedades que são necessárias ao criar o payloadCompatibleAssignmentFilter.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave do Filtro de Atribuição. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|createdDateTime|DateTimeOffset|Hora de criação do Filtro de Atribuição. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|lastModifiedDateTime|DateTimeOffset|Última hora modificada do Filtro de Atribuição. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|displayName|Cadeia de caracteres|DisplayName do Filtro de Atribuição. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|description|Cadeia de caracteres|Descrição do Filtro de Atribuição. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|plataforma|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|Tipo de plataforma dos dispositivos nos quais o Filtro de Atribuição será aplicável. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md). Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|rule|Cadeia de caracteres|Definição de regra do Filtro de Atribuição. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|roleScopeTags|Coleção de cadeias de caracteres|RoleScopeTags do Filtro de Atribuição. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|payloadType|[assignmentFilterPayloadType](../resources/intune-policyset-assignmentfilterpayloadtype.md)|PayloadType do Filtro de Atribuição. Os valores possíveis são: `notSet` e `enrollmentRestrictions`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/assignmentFilters
Content-type: application/json
Content-length: 313

{
  "@odata.type": "#microsoft.graph.payloadCompatibleAssignmentFilter",
  "displayName": "Display Name value",
  "description": "Description value",
  "platform": "androidForWork",
  "rule": "Rule value",
  "roleScopeTags": [
    "Role Scope Tags value"
  ],
  "payloadType": "enrollmentRestrictions"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 485

{
  "@odata.type": "#microsoft.graph.payloadCompatibleAssignmentFilter",
  "id": "6d189738-9738-6d18-3897-186d3897186d",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "platform": "androidForWork",
  "rule": "Rule value",
  "roleScopeTags": [
    "Role Scope Tags value"
  ],
  "payloadType": "enrollmentRestrictions"
}
```




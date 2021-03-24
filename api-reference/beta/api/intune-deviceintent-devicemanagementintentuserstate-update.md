---
title: Atualizar deviceManagementIntentUserState
description: Atualize as propriedades de um objeto deviceManagementIntentUserState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 223a10e2a46f650e3d390611380bf6c74073b560
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132006"
---
# <a name="update-devicemanagementintentuserstate"></a>Atualizar deviceManagementIntentUserState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto deviceManagementIntentUserState.](../resources/intune-deviceintent-devicemanagementintentuserstate.md)

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
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementIntentUserState.](../resources/intune-deviceintent-devicemanagementintentuserstate.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID|
|userPrincipalName|Cadeia de caracteres|O nome principal do usuário que está sendo relatado em um dispositivo|
|userName|Cadeia de caracteres|O nome de usuário que está sendo relatado em um dispositivo|
|deviceCount|Int32|Contagem de dispositivos que pertencem a um usuário para uma intenção|
|lastReportedDateTime|DateTimeOffset|Data da última modificação de um relatório de intenção|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Estado do usuário para uma intenção. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceCount": 11,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "0201286a-286a-0201-6a28-01026a280102",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceCount": 11,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable"
}
```





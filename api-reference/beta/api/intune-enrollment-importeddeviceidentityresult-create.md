---
title: Criar importedDeviceIdentityResult
description: Criar um novo objeto importedDeviceIdentityResult.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1ebe19bc2ac812502df0f09967c3d404b126644f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532748"
---
# <a name="create-importeddeviceidentityresult"></a>Criar importedDeviceIdentityResult

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto importedDeviceIdentityResult.

A tabela a seguir mostra as propriedades que são necessárias ao criar importedDeviceIdentityResult.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID da identidade de dispositivo importada herdada de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentifier|String|Identificador de dispositivo imPortado herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Tipo de identidade de dispositivo imPortado herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md). Os valores possíveis são: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação da descrição herdadas de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|createdDateTime|DateTimeOffset|Data e hora de criação do dispositivo herdadas de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|lastContactedDateTime|DateTimeOffset|Data e hora do último contato do dispositivo herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|description|String|A descrição do dispositivo herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|enrollmentid|[enrollmentid](../resources/intune-enrollment-enrollmentstate.md)|O estado do dispositivo no Intune herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md). Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|[plataforma](../resources/intune-enrollment-platform.md)|A plataforma do dispositivo. Herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md). Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Booliano|Status da identidade do dispositivo importado|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
Content-type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```






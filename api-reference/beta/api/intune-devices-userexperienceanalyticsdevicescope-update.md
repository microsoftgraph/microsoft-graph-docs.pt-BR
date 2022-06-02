---
title: Atualizar userExperienceAnalyticsDeviceScope
description: Atualize as propriedades de um objeto userExperienceAnalyticsDeviceScope.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 71f540448a2078a0af54e68205dfeff42bc35992
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858433"
---
# <a name="update-userexperienceanalyticsdevicescope"></a>Atualizar userExperienceAnalyticsDeviceScope

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceScope
PATCH /deviceManagement/userExperienceAnalyticsDeviceScopes/{userExperienceAnalyticsDeviceScopeId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo para a configuração de escopo do dispositivo.|
|deviceScopeName|String|O nome da configuração de escopo do dispositivo de análise de experiência do usuário.|
|ownerId|String|O identificador exclusivo da pessoa (administrador) que criou a configuração de escopo do dispositivo.|
|isBuiltIn|Booliano|Indica se a configuração de escopo do dispositivo é interna ou personalizada. Quando TRUE, a configuração de escopo do dispositivo é interna. Quando FALSE, a configuração de escopo do dispositivo é personalizada. O valor padrão é FALSE.|
|enabled|Boolean|Indica se um escopo de dispositivo está habilitado ou desabilitado. Quando TRUE, o escopo do dispositivo é habilitado. Quando FALSE, o escopo do dispositivo é desabilitado. O valor padrão é FALSE.|
|status|[deviceScopeStatus](../resources/intune-devices-devicescopestatus.md)|Indica o status do escopo do dispositivo depois que o escopo do dispositivo foi habilitado. Os valores possíveis são: none, computing, insufficientData ou completed. O valor padrão é none. Os valores possíveis são: `none`, `computing`, `insufficientData`, `completed`, `unknownFutureValue`.|
|parâmetro|[deviceScopeParameter](../resources/intune-devices-devicescopeparameter.md)|Parâmetro de configuração do escopo do dispositivo. Ele será estendido no futuro para adicionar mais parâmetros. Por exemplo: o parâmetro de escopo do dispositivo pode ser versão do sistema operacional, Tipo de Disco, Fabricante do dispositivo, modelo de dispositivo ou marca de escopo. Valor padrão: scopeTag. Os valores possíveis são: `none`, `scopeTag`, `unknownFutureValue`.|
|operator|[deviceScopeOperator](../resources/intune-devices-devicescopeoperator.md)|Operador de consulta de configuração do escopo do dispositivo. Os valores possíveis são: equals, notEquals, contains, notContains, greaterThan, lessThan. Valor padrão: igual a. Os valores possíveis são: `none`, `equals`, `unknownFutureValue`.|
|valueObjectId|String|O identificador exclusivo para uma ID de marca de escopo de dispositivo de usuário usada para a criação da configuração de escopo do dispositivo.|
|value|Cadeia de caracteres|O valor da cláusula de consulta de configuração do escopo do dispositivo.|
|createdDateTime|DateTimeOffset|Indica a data e a hora de criação para o escopo do dispositivo personalizado.|
|lastModifiedDateTime|DateTimeOffset|Indica a data e a hora da última atualização para o escopo do dispositivo personalizado.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScope
Content-type: application/json
Content-length: 350

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScope",
  "deviceScopeName": "Device Scope Name value",
  "ownerId": "Owner Id value",
  "isBuiltIn": true,
  "enabled": true,
  "status": "computing",
  "parameter": "scopeTag",
  "operator": "equals",
  "valueObjectId": "Value Object Id value",
  "value": "Value value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 522

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScope",
  "id": "936b0460-0460-936b-6004-6b9360046b93",
  "deviceScopeName": "Device Scope Name value",
  "ownerId": "Owner Id value",
  "isBuiltIn": true,
  "enabled": true,
  "status": "computing",
  "parameter": "scopeTag",
  "operator": "equals",
  "valueObjectId": "Value Object Id value",
  "value": "Value value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





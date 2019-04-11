---
title: Atualizar securityBaselineSettingState
description: Atualiza as propriedades de um objeto securityBaselineSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c65f3c49159f6025ae32ee9a12c7acc395742509
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787740"
---
# <a name="update-securitybaselinesettingstate"></a>Atualizar securityBaselineSettingState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualiza as propriedades de um objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .

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
PATCH /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da entidade|
|settingName|Cadeia de caracteres|O nome da configuração que está sendo relatado|
|state|[securityBaselineComplianceState](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|O estado de conformidade da configuração da linha de base de segurança. Os valores possíveis são: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.|
|settingCategoryId|Cadeia de caracteres|A ID da categoria de configuração à qual essa configuração pertence|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "settingName": "Setting Name value",
  "state": "secure",
  "settingCategoryId": "Setting Category Id value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "id": "798e520d-520d-798e-0d52-8e790d528e79",
  "settingName": "Setting Name value",
  "state": "secure",
  "settingCategoryId": "Setting Category Id value"
}
```




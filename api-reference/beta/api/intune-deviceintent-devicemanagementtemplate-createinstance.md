---
title: ação createInstance
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: babd7aa6a9f0fe5d62e0d62bb8c9657d81e3cc0e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33915997"
---
# <a name="createinstance-action"></a>ação createInstance

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

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
POST /deviceManagement/templates/{deviceManagementTemplateId}/createInstance
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}/createInstance
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Ainda não documentado|
|description|String|Ainda não documentado|
|settingsDelta|coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Ainda não documentado|



## <a name="response"></a>Resposta
Se tiver êxito, esta ação retornará `200 OK` um código de resposta e um [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/createInstance

Content-type: application/json
Content-length: 336

{
  "displayName": "Display Name value",
  "description": "Description value",
  "settingsDelta": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
      "id": "d68168e1-68e1-d681-e168-81d6e16881d6",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 350

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntent",
    "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
    "displayName": "Display Name value",
    "description": "Description value",
    "isAssigned": true,
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "templateId": "Template Id value"
  }
}
```





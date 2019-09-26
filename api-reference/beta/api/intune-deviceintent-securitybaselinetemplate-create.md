---
title: Criar securityBaselineTemplate
description: Criar um novo objeto securityBaselineTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9337b5e9a5108c8dd26cb08287d42406c5a68794
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188826"
---
# <a name="create-securitybaselinetemplate"></a>Criar securityBaselineTemplate

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
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
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto securityBaselineTemplate.

A tabela a seguir mostra as propriedades que são necessárias ao criar securityBaselineTemplate.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do modelo herdada de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|displayName|String|O nome de exibição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|descrição|String|A descrição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|versionInfo|String|As informações de versão do modelo herdadas de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|preterido|Booliano|O modelo é preterido ou não. Os propósitos não podem ser criados a partir de um modelo preterido. Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|intentCount|Int32|Número de tentativas criadas a partir deste modelo. Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|templateType|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|O tipo do modelo. Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md). Os possíveis valores são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`.|
|publishedDateTime|DateTimeOffset|Quando o modelo foi publicado herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 383

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```





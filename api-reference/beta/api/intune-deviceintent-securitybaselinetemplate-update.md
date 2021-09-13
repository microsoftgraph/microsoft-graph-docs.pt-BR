---
title: Atualizar securityBaselineTemplate
description: Atualize as propriedades de um objeto securityBaselineTemplate.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d7d51e40b96e2dfbb889f5676d8ebca5bfffcc5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59042499"
---
# <a name="update-securitybaselinetemplate"></a>Atualizar securityBaselineTemplate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)

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
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do modelo Herdada [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|displayName|Cadeia de caracteres|O nome de exibição do modelo Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|description|Cadeia de caracteres|Descrição do modelo Herdada de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|versionInfo|Cadeia de Caracteres|Informações de versão do modelo Herdadas de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|isDeprecated|Boleano|O modelo está preterido ou não. As intenções não podem ser criadas a partir de um modelo preterido. Herdado [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|intentCount|Int32|Número de Intenções criadas a partir deste modelo. Herdado [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|templateType|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|O tipo do modelo. Herdado [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md). Os valores possíveis são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.|
|platformType|[policyPlatformType](../resources/intune-deviceintent-policyplatformtype.md)|A plataforma do modelo. Herdado [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md). Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.|
|templateSubtype|[deviceManagementTemplateSubtype](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|O subtipo do modelo. Herdado [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md). Os valores possíveis são: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.|
|publishedDateTime|DateTimeOffset|Quando o modelo foi publicado Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "templateSubtype": "firewall",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 454

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "templateSubtype": "firewall",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```




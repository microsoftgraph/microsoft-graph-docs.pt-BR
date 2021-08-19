---
title: Criar deviceManagementConfigurationPolicyTemplate
description: Crie um novo objeto deviceManagementConfigurationPolicyTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b2ec39aeb98819c2f417b4dce7b8874d27fb8e65
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262957"
---
# <a name="create-devicemanagementconfigurationpolicytemplate"></a>Criar deviceManagementConfigurationPolicyTemplate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto deviceManagementConfigurationPolicyTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicyTemplates
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementConfigurationPolicyTemplate.

A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationPolicyTemplate.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave do documento do modelo, composta por BaseId e Version. Gerado automaticamente.|
|baseId|Cadeia de caracteres|Identificador de base de modelos|
|versão|Int32|Versão do modelo. Valores válidos 1 a 2147483647. Essa propriedade é somente leitura.|
|displayName|Cadeia de caracteres|Nome de exibição do modelo|
|description|Cadeia de caracteres|Descrição do modelo|
|displayVersion|Cadeia de caracteres|Descrição da versão do modelo|
|lifecycleState|[deviceManagementTemplateLifecycleState](../resources/intune-deviceconfigv2-devicemanagementtemplatelifecyclestate.md)|Indique o estado atual do modelo de ciclo de vida. Os possíveis valores são: `invalid`, `draft`, `active`, `superseded`, `deprecated`, `retired`.|
|plataformas|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Plataformas para este modelo. Os valores possíveis são: `none`, `macOS`, `windows10X`, `windows10`.|
|technologies|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Tecnologias para este modelo. Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.|
|templateFamily|[deviceManagementConfigurationTemplateFamily](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|TemplateFamily para este modelo. Os valores possíveis são: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.|
|allowUnmanagedSettings|Boolean|Permitir modelos de configuração nãomanageados|
|settingTemplateCount|Int32|Número de modelos de configuração. Valores válidos de 0 a 2147483647. Essa propriedade é somente leitura.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicyTemplates
Content-type: application/json
Content-length: 453

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
  "baseId": "Base Id value",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "displayVersion": "Display Version value",
  "lifecycleState": "draft",
  "platforms": "macOS",
  "technologies": "mdm",
  "templateFamily": "endpointSecurityAntivirus",
  "allowUnmanagedSettings": true,
  "settingTemplateCount": 4
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 502

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
  "id": "424ddb9a-db9a-424d-9adb-4d429adb4d42",
  "baseId": "Base Id value",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "displayVersion": "Display Version value",
  "lifecycleState": "draft",
  "platforms": "macOS",
  "technologies": "mdm",
  "templateFamily": "endpointSecurityAntivirus",
  "allowUnmanagedSettings": true,
  "settingTemplateCount": 4
}
```





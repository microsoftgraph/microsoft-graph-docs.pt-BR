---
title: Criar deviceManagementConfigurationSettingTemplate
description: Crie um novo objeto deviceManagementConfigurationSettingTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 38b9a34107c5262ea5dab7b2dd350904e9c8d992
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346882"
---
# <a name="create-devicemanagementconfigurationsettingtemplate"></a>Criar deviceManagementConfigurationSettingTemplate

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)

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
POST /deviceManagement/templateSettings
POST /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementConfigurationSettingTemplate.

A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationSettingTemplate.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave deste modelo de configuração no modelo de política que o contém. Gerado automaticamente.|
|settingInstanceTemplate|[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|Modelo de instância de configuração|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templateSettings
Content-type: application/json
Content-length: 784

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingTemplate",
  "settingInstanceTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
    "settingInstanceTemplateId": "Setting Instance Template Id value",
    "settingDefinitionId": "Setting Definition Id value",
    "isRequired": true,
    "simpleSettingValueTemplate": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
      "settingValueTemplateId": "Setting Value Template Id value",
      "defaultValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
        "constantValue": "Constant Value value"
      }
    }
  }
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 833

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingTemplate",
  "id": "203fd028-d028-203f-28d0-3f2028d03f20",
  "settingInstanceTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
    "settingInstanceTemplateId": "Setting Instance Template Id value",
    "settingDefinitionId": "Setting Definition Id value",
    "isRequired": true,
    "simpleSettingValueTemplate": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
      "settingValueTemplateId": "Setting Value Template Id value",
      "defaultValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
        "constantValue": "Constant Value value"
      }
    }
  }
}
```





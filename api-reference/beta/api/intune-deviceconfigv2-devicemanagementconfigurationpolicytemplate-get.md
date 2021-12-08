---
title: Obter deviceManagementConfigurationPolicyTemplate
description: Leia propriedades e relações do objeto deviceManagementConfigurationPolicyTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 56f6541ed3cd86d44ea7edafb3d416ef875c847d
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342213"
---
# <a name="get-devicemanagementconfigurationpolicytemplate"></a>Obter deviceManagementConfigurationPolicyTemplate

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Leia propriedades e relações do [objeto deviceManagementConfigurationPolicyTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 549

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
    "id": "424ddb9a-db9a-424d-9adb-4d429adb4d42",
    "baseId": "Base Id value",
    "version": 7,
    "displayName": "Display Name value",
    "description": "Description value",
    "displayVersion": "Display Version value",
    "lifecycleState": "draft",
    "platforms": "android",
    "technologies": "mdm",
    "templateFamily": "endpointSecurityAntivirus",
    "allowUnmanagedSettings": true,
    "settingTemplateCount": 4
  }
}
```





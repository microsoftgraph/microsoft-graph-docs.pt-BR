---
title: Atualizar deviceManagementCompliancePolicy
description: Atualize as propriedades de um objeto deviceManagementCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c5f4d942d6b08052387a4c40fdb71acf1385e72d
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346483"
---
# <a name="update-devicemanagementcompliancepolicy"></a>Atualizar deviceManagementCompliancePolicy

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto deviceManagementCompliancePolicy.](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)

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
PATCH /deviceManagement/compliancePolicies/{deviceManagementCompliancePolicyId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementCompliancePolicy.](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave do documento de política. Gerado automaticamente.|
|nome|String|Nome da política|
|descrição|String|Descrição da política|
|plataformas|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Plataformas para essa política. Os possíveis valores são: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`.|
|technologies|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Tecnologias para essa política. Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|Data e hora de criação de política. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação da política. Essa propriedade é somente leitura.|
|settingCount|Int32|Número de configurações. Essa propriedade é somente leitura.|
|creationSource|String|Fonte de criação de política|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância entity.|
|isAssigned|Boolean|Status da atribuição de política. Essa propriedade é somente leitura.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/compliancePolicies/{deviceManagementCompliancePolicyId}
Content-type: application/json
Content-length: 345

{
  "@odata.type": "#microsoft.graph.deviceManagementCompliancePolicy",
  "name": "Name value",
  "description": "Description value",
  "platforms": "android",
  "technologies": "mdm",
  "settingCount": 12,
  "creationSource": "Creation Source value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isAssigned": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 517

{
  "@odata.type": "#microsoft.graph.deviceManagementCompliancePolicy",
  "id": "1db4aeb3-aeb3-1db4-b3ae-b41db3aeb41d",
  "name": "Name value",
  "description": "Description value",
  "platforms": "android",
  "technologies": "mdm",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "settingCount": 12,
  "creationSource": "Creation Source value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isAssigned": true
}
```





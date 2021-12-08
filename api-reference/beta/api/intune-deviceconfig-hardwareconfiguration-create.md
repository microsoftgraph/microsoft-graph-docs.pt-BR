---
title: Criar hardwareConfiguration
description: Crie um novo objeto hardwareConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97b4d40b7bd99b70a46f7d6c929ff2209ef1821d
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345334"
---
# <a name="create-hardwareconfiguration"></a>Criar hardwareConfiguration

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto hardwareConfiguration.](../resources/intune-deviceconfig-hardwareconfiguration.md)

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
POST /deviceManagement/hardwareConfigurations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto hardwareConfiguration.

A tabela a seguir mostra as propriedades que são necessárias ao criar o hardwareConfiguration.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para a configuração de hardware|
|versão|Int32|Versão da configuração de hardware|
|displayName|String|Nome da configuração de hardware|
|descrição|String|Descrição da configuração de hardware|
|createdDateTime|DateTimeOffset|Data e hora de quando a configuração de hardware foi criada. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|Data e hora de quando a configuração de hardware foi modificada. Essa propriedade é somente leitura.|
|fileName|String|Nome do arquivo da configuração de hardware|
|configurationFileContent|Binária|Conteúdo do arquivo da configuração de hardware|
|hardwareConfigurationFormat|[hardwareConfigurationFormat](../resources/intune-deviceconfig-hardwareconfigurationformat.md)|Tipo Oem da configuração de hardware. Os valores possíveis são: `dell`, `surface`, `surfaceDock`.|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de IDs de marca de escopo para a configuração de hardware|
|perDevicePasswordDisabled|Booliano|Um valor que indica se por pasword devcive desabilitado|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/hardwareConfigurations
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.hardwareConfiguration",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "fileName": "File Name value",
  "configurationFileContent": "Y29uZmlndXJhdGlvbkZpbGVDb250ZW50",
  "hardwareConfigurationFormat": "surface",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "perDevicePasswordDisabled": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 577

{
  "@odata.type": "#microsoft.graph.hardwareConfiguration",
  "id": "da410f27-0f27-da41-270f-41da270f41da",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "fileName": "File Name value",
  "configurationFileContent": "Y29uZmlndXJhdGlvbkZpbGVDb250ZW50",
  "hardwareConfigurationFormat": "surface",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "perDevicePasswordDisabled": true
}
```





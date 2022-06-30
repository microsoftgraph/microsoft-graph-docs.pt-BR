---
title: Atualizar deviceManagementDerivedCredentialSettings
description: Atualize as propriedades de um objeto deviceManagementDerivedCredentialSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8e54f3d19413e64a359ff0c22bd311fbfc07dacc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436663"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a>Atualizar deviceManagementDerivedCredentialSettings

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)||
| &nbsp; &nbsp; **Configuração do dispositivo** | DeviceManagementConfiguration.ReadWrite.All|
| &nbsp;&nbsp; **Política de Acesso a Recursos** | DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo||
| &nbsp; &nbsp; **Configuração do dispositivo** | DeviceManagementConfiguration.ReadWrite.All|
| &nbsp;&nbsp; **Política de Acesso a Recursos** | DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosDerivedCredentialAuthenticationConfiguration/derivedCredentialSettings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para a credencial derivada|
|**Política de RA**|
|helpUrl|Cadeia de caracteres|A URL que será acessível aos usuários finais à medida que eles recuperam uma credencial derivada usando o Portal da Empresa.|
|displayName|Cadeia de caracteres|O nome de exibição do perfil.|
|Emissor|[deviceManagementDerivedCredentialIssuer](../resources/intune-shared-devicemanagementderivedcredentialissuer.md)|O provedor de credenciais derivadas a ser usado. Os valores possíveis são: `intercede`, `entrustDatacard`, `purebred`.|
|Notificationtype|[deviceManagementDerivedCredentialNotificationType](../resources/intune-shared-devicemanagementderivedcredentialnotificationtype.md)|Os métodos usados para informar o usuário final para abrir Portal da Empresa fornecer perfis de Wi-Fi, VPN ou email que usam certificados para o dispositivo. Os valores possíveis são: `none`, `companyPortal`, `email`.|


## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 83

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc"
}
```








---
title: Criar windows10SecureAssessmentConfiguration
description: Cria um novo objeto windows10SecureAssessmentConfiguration.
author: tfitzmac
ms.openlocfilehash: 21964a84ac046adb7a27c511319a903ff2ab50f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308348"
---
# <a name="create-windows10secureassessmentconfiguration"></a>Criar windows10SecureAssessmentConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Cria um novo objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).
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
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Accept|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto windows10SecureAssessmentConfiguration.

A tabela a seguir mostra as propriedades que são necessárias ao criar windows10SecureAssessmentConfiguration.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|Lista de escopo marcas para essa instância da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo. Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|launchUri|String|Link da URL para uma avaliação que é carregada automaticamente quando o navegador de avaliação segura é iniciado. Ele precisa ser uma URL válida (http\[s\]://msdn.microsoft.com/).|
|configurationAccount|String|A conta usada para configurar o dispositivo Windows para realizar o teste. O usuário pode ser uma conta de domínio (domínio\usuário), uma conta do AAD (nomedeusuário@locatário.com) ou uma conta local (nomedeusuário).|
|configurationAccountType|[secureAssessmentAccountType](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|O tipo de conta usado para por ConfigurationAccount. Os valores possíveis são: `azureADAccount`, `domainAccount`, `localAccount`.|
|allowPrinting|Boolean|Indica se o aplicativo deve ou não ter permissão de impressão durante o teste.|
|allowScreenCapture|Boolean|Indica se a capacidade de captura de tela deve ou não ser permitida durante um teste.|
|allowTextSuggestion|Boolean|Indica se sugestões de texto devem ou não ser permitidas durante o teste.|



## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 563

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 671

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```






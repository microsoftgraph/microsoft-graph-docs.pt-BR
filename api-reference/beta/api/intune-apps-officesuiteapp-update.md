---
title: Atualizar officeSuiteApp
description: Atualize as propriedades de um objeto officeSuiteApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a6b286c53cfcd6d6b93a91ea63cb1e693e168e57
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405314"
---
# <a name="update-officesuiteapp"></a>Atualizar officeSuiteApp

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Atualize as propriedades de um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .

A tabela a seguir mostra as propriedades que são necessárias quando você cria o [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|String|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|description|String|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publisher|String|O publicador do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|String|A URL da declaração de privacidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|informationUrl|String|A URL de informações adicionais. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|String|O proprietário do conteúdo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|O desenvolvedor do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|Observações|String|Anotações para o aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|uploadState|Int32|O estado de carregamento. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|O estado de publicação para o aplicativo. O aplicativo não pode ser assinado, a menos que ele seja publicado. Herdada do [mobileApp](../resources/intune-apps-mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|O valor que indica se o aplicativo é atribuído a pelo menos um grupo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|roleScopeTagIds|String collection|Lista de ids de marca de escopo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|autoAcceptEula|Boolean|O valor para aceitar o EULA automaticamente no dispositivo do usuário final.|
|productIds|coleção [officeProductId](../resources/intune-apps-officeproductid.md)|As Ids de produto que representam a SKU do pacote Office365. Os valores possíveis são: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.|
|excludedApps|[excludedApps](../resources/intune-apps-excludedapps.md)|A propriedade para representar os aplicativos que são excluídos do produto selecionado Office365 ID.|
|useSharedComputerActivation|Boolean|A propriedade para representar que se a ativação do computador compartilhado é usada não para o pacote do app Office365.|
|updateChannel|[officeUpdateChannel](../resources/intune-apps-officeupdatechannel.md)|A propriedade para representar o canal de atualização Office365. Os valores possíveis são: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.|
|officePlatformArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|A propriedade para representar a versão do pacote de aplicativo Office365. Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|localesToInstall|String collection|A propriedade para representar as localidades que são instaladas quando os aplicativos a partir Office365 está instalado. Ele usa 6033 standard do RFC. REF:https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx|
|installProgressDisplayLevel|[officeSuiteInstallProgressDisplayLevel](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|Para especificar o nível de exibição para a interface de usuário de instalação de progresso da instalação no dispositivo. Os valores possíveis são: `none` e `full`.|
|shouldUninstallOlderVersionsOfOffice|Boolean|A propriedade para determinar se você desinstalar o MSI existente do Office se um pacote do app Office365 é implantado com o dispositivo ou não.|
|targetVersion|String|A propriedade para representar a versão de destino específicos para o pacote do app Office365 que deve ser permaneceu implantada nos dispositivos.|
|updateVersion|String|A propriedade para representar a versão de atualização em que a versão de destino específico está disponível para o pacote de aplicativo Office365.|
|officeConfigurationXml|Binária|A propriedade para representar o arquivo de configuração XML que pode ser especificado para o Office ProPlus Apps. Tem precedência sobre todas as outras propriedades. Quando presente, o arquivo de configuração XML será usado para criar o aplicativo.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1552

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1724

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "id": "9b263b46-3b46-9b26-463b-269b463b269b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```





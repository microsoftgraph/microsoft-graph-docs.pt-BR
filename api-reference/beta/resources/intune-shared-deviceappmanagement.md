---
title: Tipo de recurso deviceAppManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6fb0dd517a340832b90eb70026100c4da0cf0f51
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404054"
---
# <a name="deviceappmanagement-resource-type"></a>Tipo de recurso deviceAppManagement

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceAppManagement](../api/intune-shared-deviceappmanagement-get.md)|Ler propriedades e relações de objetos de [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).|
|[Atualizar deviceAppManagement](../api/intune-shared-deviceappmanagement-update.md)|Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).|
|**Inclusão**|
|[Ação syncMicrosoftStoreForBusinessApps](../api/intune-shared-deviceappmanagement-syncmicrosoftstoreforbusinessapps.md)|Nenhum|Sincroniza a conta do Intune com o Microsoft Store para Empresas|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|**Inclusão**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.|
|microsoftStoreForBusinessLanguage|String|As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas. Culturas específicas de um país/região. Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes). O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166. Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|A última vez em uma sincronização de aplicativo na Microsoft Store para Empresas foi concluída.|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.|
|microsoftStoreForBusinessPortalSelection|[microsoftStoreForBusinessPortalSelectionOptions](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|As informações do portal de usuário final são usadas para sincronizar os aplicativos do Microsoft Store for Business para Intune Portal da empresa. Existem três opções para selecionar \['Somente para portal da empresa', 'Empresa portal e particular armazenar', 'Somente armazenamento particular'\]. Os valores possíveis são: `none`, `companyPortal`, `privateStore`.|

## <a name="relationships"></a>Relacionamentos
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Aplicativos**|
|enterpriseCodeSigningCertificates|coleção [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|O código de empresa do Windows certificado de assinatura.|
|iosLobAppProvisioningConfigurations|coleção [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|Configurações de provisionamento de aplicativos de Lob IOS.|
|mobileAppCategories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|As categorias dos aplicativos móveis.|
|mobileAppConfigurations|Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|As configurações de aplicativos móveis de gerenciamento de dispositivos.|
|mobileApps|Coleção [mobileApp](../resources/intune-apps-mobileapp.md)|Os aplicativos móveis.|
|symantecCodeSigningCertificate|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|O código de Symantec WinPhone certificado de assinatura.|
|**Manuais**|
|managedEBooks|Conjunto [managedEBook](../resources/intune-books-managedebook.md)|Livro eletrônico gerenciado.|
|managedEBookCategories|coleção [managedEBookCategory](../resources/intune-books-managedebookcategory.md)|As categorias de eBook móvel.|
|**Gerenciamento de dispositivos**|
|windowsManagementApp|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Aplicativo de gerenciamento do Windows.|
|**Gerenciamento de aplicativo móvel (MAM)**|
|androidManagedAppProtections|Coleção [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md)|Políticas de aplicativos gerenciados para Android.|
|defaultManagedAppProtections|Coleção [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Políticas de aplicativos gerenciados padrão.|
|iosManagedAppProtections|Coleção [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)|Políticas de aplicativos gerenciados para iOS.|
|managedAppPolicies|Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Políticas de aplicativos gerenciados.|
|managedAppRegistrations|Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Os registros de aplicativos gerenciados.|
|managedAppStatuses|Coleção [managedAppStatus](../resources/intune-mam-managedappstatus.md)|Os status de aplicativos gerenciados.|
|mdmWindowsInformationProtectionPolicies|Coleção [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|Proteção de informações do Windows para aplicativos em execução em dispositivos que estão registrados no MDM.|
|targetedManagedAppConfigurations|Coleção [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)|Configurações de aplicativos gerenciados direcionadas.|
|windowsInformationProtectionPolicies|Coleção [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)|Proteção de informações do Windows para aplicativos em execução em dispositivos que não estão registrados no MDM.|
|**Inclusão**|
|sideLoadingKeys|coleção [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Teclas Carregando lado que são necessários para o Windows 8 e 8.1 instalação de aplicativos.|
|vppTokens|Coleção de [vppToken](../resources/intune-onboarding-vpptoken.md)|Lista de tokens Vpp desta organização.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.  Observe que isso é apenas um exemplo; respostas de consulta às consultas reais irá conter as propriedades apropriadas para o contexto.  
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "String (timestamp)",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "String",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "String (timestamp)"
}
```




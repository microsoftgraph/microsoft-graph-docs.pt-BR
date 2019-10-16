---
title: Tipo de recurso deviceAppManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b9a5b072c5aa71da4038b66597eae5d796b14d0d
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539159"
---
# <a name="deviceappmanagement-resource-type"></a>Tipo de recurso deviceAppManagement

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceAppManagement](../api/intune-shared-deviceappmanagement-get.md)|Ler propriedades e relações de objetos de [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).|
|[Atualizar deviceAppManagement](../api/intune-shared-deviceappmanagement-update.md)|Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).|
|**Integração**|
|[Ação syncMicrosoftStoreForBusinessApps](../api/intune-shared-deviceappmanagement-syncmicrosoftstoreforbusinessapps.md)|Nenhum|Sincroniza a conta do Intune com o Microsoft Store para Empresas|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|**Integração**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.|
|microsoftStoreForBusinessLanguage|String|As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas. Culturas específicas de um país/região. Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes). O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166. Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|A última vez em uma sincronização de aplicativo na Microsoft Store para Empresas foi concluída.|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.|
|microsoftStoreForBusinessPortalSelection|[microsoftStoreForBusinessPortalSelectionOptions](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|As informações do portal do usuário final são usadas para sincronizar aplicativos da Microsoft Store para empresas com o portal da empresa do Intune. Há três opções a serem escolhidas \[em "somente portal da empresa", "portal da empresa e repositório privado", "somente\]repositório privado". Os valores possíveis são: `none`, `companyPortal`, `privateStore`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Apps**|
|enterpriseCodeSigningCertificates|coleção [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|O certificado de assinatura de código do Windows Enterprise.|
|iosLobAppProvisioningConfigurations|coleção [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|As configurações de provisionamento do aplicativo LOB do IOS.|
|mobileAppCategories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|As categorias dos aplicativos móveis.|
|mobileAppConfigurations|Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|As configurações de aplicativos móveis de gerenciamento de dispositivos.|
|mobileApps|Coleção [mobileApp](../resources/intune-shared-mobileapp.md)|Os aplicativos móveis.|
|symantecCodeSigningCertificate|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|O certificado de assinatura de código Symantec do WinPhone.|
|**Deprecia**|
|managedEBooks|Conjunto [managedEBook](../resources/intune-books-managedebook.md)|Livro eletrônico gerenciado.|
|managedEBookCategories|coleção [managedEBookCategory](../resources/intune-books-managedebookcategory.md)|As categorias do eBook móvel.|
|**Gerenciamento de dispositivos**|
|windowsManagementApp|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Aplicativo de gerenciamento do Windows.|
|**Gerenciamento de aplicativo móvel (GAM)**|
|androidManagedAppProtections|Coleção [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md)|Políticas de aplicativos gerenciados para Android.|
|defaultManagedAppProtections|Coleção [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Políticas de aplicativos gerenciados padrão.|
|iosManagedAppProtections|Coleção [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md)|Políticas de aplicativos gerenciados para iOS.|
|managedAppPolicies|Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Políticas de aplicativos gerenciados.|
|managedAppRegistrations|Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Os registros de aplicativos gerenciados.|
|managedAppStatuses|Coleção [managedAppStatus](../resources/intune-mam-managedappstatus.md)|Os status de aplicativos gerenciados.|
|mdmWindowsInformationProtectionPolicies|Coleção [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md)|Proteção de informações do Windows para aplicativos em execução em dispositivos que estão registrados no MDM.|
|targetedManagedAppConfigurations|Coleção [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)|Configurações de aplicativos gerenciados direcionadas.|
|windowsInformationProtectionPolicies|Coleção [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)|Proteção de informações do Windows para aplicativos em execução em dispositivos que não estão registrados no MDM.|
|**Integração**|
|sideLoadingKeys|coleção [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Chaves de carregamento do lado necessárias para a instalação de aplicativos do Windows 8 e 8,1.|
|vppTokens|Coleção de [vppToken](../resources/intune-onboarding-vpptoken.md)|Lista de tokens Vpp desta organização.|
|**Conjunto de políticas**|
|policySets|coleção [policyset](../resources/intune-policyset-policyset.md)|O Policyset de políticas e aplicativos|
|mobileApps|Coleção [mobileApp](../resources/intune-shared-mobileapp.md)|Os aplicativos móveis.|
|targetedManagedAppConfigurations|Coleção [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)|Configurações de aplicativos gerenciados direcionadas.|
|androidManagedAppProtections|Coleção [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md)|Políticas de aplicativos gerenciados para Android.|
|iosManagedAppProtections|Coleção [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md)|Políticas de aplicativos gerenciados para iOS.|
|mdmWindowsInformationProtectionPolicies|Coleção [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md)|Proteção de informações do Windows para aplicativos em execução em dispositivos que estão registrados no MDM.|
|iosLobAppProvisioningConfigurations|coleção [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|As configurações de provisionamento do aplicativo LOB do IOS.|
|**Integração com parceiros**|
|deviceAppManagementTasks|coleção [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Tarefas de gerenciamento de aplicativos do dispositivo.|
|**Unlock**|
|wdacSupplementalPolicies|coleção [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|O conjunto de políticas suplementares do controle de aplicativos do Windows Defender.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.  Observe que este é apenas um exemplo; as respostas de consulta a consultas reais conterá as propriedades apropriadas para o contexto.  
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




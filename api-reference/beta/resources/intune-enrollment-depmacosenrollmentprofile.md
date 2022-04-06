---
title: Tipo de recurso de depMacOSEnrollmentProfile
description: O recurso DepMacOSEnrollmentProfile representa um perfil de registro do Programa de Registro de Dispositivo Apple (DEP) específico da configuração do macOS. Esse tipo de perfil deve ser atribuído aos números de série de DEP da Apple antes que os dispositivos correspondentes possam se registrar por meio de DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6f93bd3c39e76dd0b85744bcc89b0183073d3fc9
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2022
ms.locfileid: "64630677"
---
# <a name="depmacosenrollmentprofile-resource-type"></a>Tipo de recurso de depMacOSEnrollmentProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso DepMacOSEnrollmentProfile representa um perfil de registro do Programa de Registro de Dispositivo Apple (DEP) específico da configuração do macOS. Esse tipo de perfil deve ser atribuído aos números de série de DEP da Apple antes que os dispositivos correspondentes possam se registrar por meio de DEP.


Herda [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar depMacOSEnrollmentProfiles](../api/intune-enrollment-depmacosenrollmentprofile-list.md)|[Coleção de depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Listar propriedades e relações dos objetos [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .|
|[Obter depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-get.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Leia propriedades e relações do [objeto depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .|
|[Criar depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-create.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Crie um novo [objeto depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .|
|[Excluir depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-delete.md)|Nenhum|Exclui um [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).|
|[Atualizar depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-update.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Atualize as propriedades [de um objeto depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O GUID do objeto Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|Nome do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|descrição|String|Descrição do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boolean|Indica se o perfil requer autenticação de usuário Herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String|URL do ponto de extremidade de configuração a ser usada para Registro Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|Indica a autenticação com o Assistente de Instalação da Apple em vez de Portal da Empresa. Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Booleano|Indica que a Portal da Empresa é necessária em dispositivos inscritos do assistente de instalação Herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Booliano|Indica se esse é o perfil padrão Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Booliano|Modo supervisionado, True para habilitar, false caso contrário. Consulte [Registrar dispositivos no Microsoft Intune](/mem/intune/enrollment) para obter informações adicionais. Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|String|Informações do departamento de suporte Herdadas [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|isMandatory|Booleano|Indica se o perfil é obrigatório Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|locationDisabled|Booliano|Indica se o painel de configuração do serviço de local está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportPhoneNumber|String|Número de telefone de suporte Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Boolean|Indica se a opção de remoção de perfil está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|restoreBlocked|Booleano|Indica se o painel restaurar instalação está bloqueado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|appleIdDisabled|Boolean|Indica se o painel de configuração de ID da Apple está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Booleano|Indica se o painel de configuração 'Termos e Condições' está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|touchIdDisabled|Booliano|Indica se o painel de configuração de id por toque está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|applePayDisabled|Booleano|Indica se o painel de configuração de pagamento da Apple está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|siriDisabled|Booleano|Indica se o painel de configuração de siri está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Boolean|Indica se o painel de configuração de diagnósticos está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|displayToneSetupDisabled|Boolean|Indica se a tela de instalação de displaytone está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|privacyPaneDisabled|Booliano|Indica se a tela de privacidade está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|screenTimeScreenDisabled|Booliano|Indica se a configuração do tempo de tempo de tela está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|deviceNameTemplate|String|Define um padrão literal ou de nome. Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|configurationWebUrl|Booleano|URL para logon do assistente de instalação Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|registrationDisabled|Boolean|Indica se o registro está desabilitado|
|fileVaultDisabled|Booliano|Indica se o cofre de arquivos está desabilitado|
|iCloudDiagnosticsDisabled|Booliano|Indica se a tela do iCloud Analytics está desabilitada|
|passCodeDisabled|Booleano|Indica se o painel de configuração senha está desabilitado|
|zoomDisabled|Booliano|Indica se o painel de configuração de zoom está desabilitado|
|iCloudStorageDisabled|Booliano|Indica se a tela documentos e área de trabalho do iCloud está desabilitada|
|chooseYourLockScreenDisabled|Boolean|Indica se a tela documentos e área de trabalho do iCloud está desabilitada|
|accessibilityScreenDisabled|Boolean|Indica se a tela acessibilidade está desabilitada|
|autoUnlockWithWatchDisabled|Booliano|Indica se a tela UnlockWithWatch está desabilitada|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depMacOSEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "String",
  "configurationWebUrl": true,
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true,
  "accessibilityScreenDisabled": true,
  "autoUnlockWithWatchDisabled": true
}
```





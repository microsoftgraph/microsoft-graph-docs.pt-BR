---
title: tipo de recurso depEnrollmentBaseProfile
description: O recurso DepEnrollmentBaseProfile representa um perfil de registro de programa de registro de dispositivo (DEP) Apple. Esse tipo de perfil deve ser atribuído aos números de série da Apple DEP antes que os dispositivos correspondentes possam se inscrever via DEP.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0b33d4c8ed70c5391d1bc5f85761dfac6f61a76
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941657"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>tipo de recurso depEnrollmentBaseProfile

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso DepEnrollmentBaseProfile representa um perfil de registro de programa de registro de dispositivo (DEP) Apple. Esse tipo de perfil deve ser atribuído aos números de série da Apple DEP antes que os dispositivos correspondentes possam se inscrever via DEP.


Herda de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar depEnrollmentBaseProfiles](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|coleção [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Listar Propriedades e relações dos objetos [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .|
|[Obter depEnrollmentBaseProfile](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Leia as propriedades e as relações do objeto [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Booliano|Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|Cadeia de caracteres|URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|Enableauthenticationviacompanyportal foi adicionada|Booliano|Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa. Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Booliano|Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Booliano|Indica se este é o perfil padrão|
|supervisedModeEnabled|Booliano|Modo supervisionado, true para habilitar, caso contrário, false. Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.|
|supportDepartment|Cadeia de caracteres|Informações do departamento de suporte|
|passCodeDisabled|Booliano|Indica se o painel de configuração de senha está desabilitado|
|IsMandatory|Booliano|Indica se o perfil é obrigatório|
|locationDisabled|Booliano|Indica se o painel de instalação do serviço de localização está desabilitado|
|supportPhoneNumber|Cadeia de caracteres|Número de telefone de suporte|
|profileRemovalDisabled|Booliano|Indica se a opção de remoção de perfil está desabilitada|
|restoreBlocked|Booliano|Indica se o painel de configuração de restauração está bloqueado|
|appleIdDisabled|Booliano|Indica se o painel de configuração de ID da Apple está desabilitado|
|termsAndConditionsDisabled|Booliano|Indica se o painel de configuração ' termos e condições ' está desabilitado|
|touchIdDisabled|Booliano|Indica se o painel de configuração de ID de toque está desabilitado|
|applePayDisabled|Booliano|Indica se o painel de configuração de pagamento da Apple está desabilitado|
|zoomDisabled|Booliano|Indica se o painel de configuração de zoom está desabilitado|
|siriDisabled|Booliano|Indica se o painel de configuração do Siri está desabilitado|
|diagnosticsDisabled|Booliano|Indica se o painel de configuração de diagnóstico está desabilitado|
|displayToneSetupDisabled|Booliano|Indica se a tela de configuração do displaytone está desabilitada|
|privacyPaneDisabled|Booliano|Indica se a tela de privacidade está desabilitada|
|deviceNameTemplate|Cadeia de caracteres|Define um padrão literal ou de nome.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentBaseProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
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
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "deviceNameTemplate": "String"
}
```





---
title: Tipo de recurso de depEnrollmentBaseProfile
description: O recurso DepEnrollmentBaseProfile representa um perfil de registro do Programa de Registro de Dispositivo Apple (DEP). Esse tipo de perfil deve ser atribuído aos números de série de DEP da Apple antes que os dispositivos correspondentes possam se registrar por meio de DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8f381af9b3b97579bf14a2a34c00bfb9f82f8040
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60493484"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>Tipo de recurso de depEnrollmentBaseProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso DepEnrollmentBaseProfile representa um perfil de registro do Programa de Registro de Dispositivo Apple (DEP). Esse tipo de perfil deve ser atribuído aos números de série de DEP da Apple antes que os dispositivos correspondentes possam se registrar por meio de DEP.


Herda de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar depEnrollmentBaseProfiles](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|[Coleção de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Listar propriedades e relações dos [objetos depEnrollmentBaseProfile.](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|[Obter depEnrollmentBaseProfile](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Leia propriedades e relações do [objeto depEnrollmentBaseProfile.](../resources/intune-enrollment-depenrollmentbaseprofile.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Cadeia de caracteres|Nome do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|Cadeia de caracteres|Descrição do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Booliano|Indica se o perfil requer autenticação de usuário Herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|Cadeia de caracteres|URL do ponto de extremidade de configuração a ser usada para Registro Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Booliano|Indica a autenticação com o Assistente de Instalação da Apple em vez de Portal da Empresa. Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Booliano|Indica que a Portal da Empresa é necessária em dispositivos inscritos do assistente de instalação Herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Booliano|Indica se esse é o perfil padrão|
|supervisedModeEnabled|Booliano|Modo supervisionado, True para habilitar, false caso contrário. Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.|
|supportDepartment|Cadeia de caracteres|Informações do departamento de suporte|
|isMandatory|Booliano|Indica se o perfil é obrigatório|
|locationDisabled|Booliano|Indica se o painel de configuração do serviço de localização está desabilitado|
|supportPhoneNumber|Cadeia de caracteres|Número de telefone de suporte|
|profileRemovalDisabled|Booliano|Indica se a opção de remoção de perfil está desabilitada|
|restoreBlocked|Booliano|Indica se o painel restaurar instalação está bloqueado|
|appleIdDisabled|Booliano|Indica se o painel de configuração de ID da Apple está desabilitado|
|termsAndConditionsDisabled|Booliano|Indica se o painel de configuração 'Termos e Condições' está desabilitado|
|touchIdDisabled|Booliano|Indica se o painel de configuração de ID por toque está desabilitado|
|applePayDisabled|Booliano|Indica se o painel de configuração de pagamento da Apple está desabilitado|
|siriDisabled|Booliano|Indica se o painel de configuração de siri está desabilitado|
|diagnosticsDisabled|Booliano|Indica se o painel de configuração de diagnósticos está desabilitado|
|displayToneSetupDisabled|Booliano|Indica se a tela de instalação de displaytone está desabilitada|
|privacyPaneDisabled|Booliano|Indica se a tela de privacidade está desabilitada|
|screenTimeScreenDisabled|Booliano|Indica se a configuração do tempo de tempo de tela está desabilitada|
|deviceNameTemplate|Cadeia de caracteres|Define um padrão literal ou de nome.|
|configurationWebUrl|Booliano|URL para logon do assistente de instalação|

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
  "configurationWebUrl": true
}
```




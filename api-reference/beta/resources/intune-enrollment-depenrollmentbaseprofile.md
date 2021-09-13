---
title: Tipo de recurso de depEnrollmentBaseProfile
description: O recurso DepEnrollmentBaseProfile representa um perfil de registro do Programa de Registro de Dispositivo Apple (DEP). Esse tipo de perfil deve ser atribuído aos números de série de DEP da Apple antes que os dispositivos correspondentes possam se registrar por meio de DEP.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 999b00260443c9c7efdc8c2d84a131f92b4ad35d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091234"
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
|requiresUserAuthentication|Boleano|Indica se o perfil requer autenticação de usuário Herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|Cadeia de Caracteres|URL do ponto de extremidade de configuração a ser usada para Registro Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boleano|Indica a autenticação com o Assistente de Instalação da Apple em vez de Portal da Empresa. Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boleano|Indica que a Portal da Empresa é necessária em dispositivos inscritos do assistente de instalação Herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Booliano|Indica se esse é o perfil padrão|
|supervisedModeEnabled|Boleano|Modo supervisionado, True para habilitar, false caso contrário. Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.|
|supportDepartment|Cadeia de Caracteres|Informações do departamento de suporte|
|isMandatory|Boleano|Indica se o perfil é obrigatório|
|locationDisabled|Boleano|Indica se o painel de configuração do serviço de localização está desabilitado|
|supportPhoneNumber|Cadeia de Caracteres|Número de telefone de suporte|
|profileRemovalDisabled|Boleano|Indica se a opção de remoção de perfil está desabilitada|
|restoreBlocked|Boleano|Indica se o painel restaurar instalação está bloqueado|
|appleIdDisabled|Boleano|Indica se o painel de configuração de ID da Apple está desabilitado|
|termsAndConditionsDisabled|Boleano|Indica se o painel de configuração 'Termos e Condições' está desabilitado|
|touchIdDisabled|Boleano|Indica se o painel de configuração de ID por toque está desabilitado|
|applePayDisabled|Boleano|Indica se o painel de configuração de pagamento da Apple está desabilitado|
|siriDisabled|Boleano|Indica se o painel de configuração de siri está desabilitado|
|diagnosticsDisabled|Boleano|Indica se o painel de configuração de diagnósticos está desabilitado|
|displayToneSetupDisabled|Boleano|Indica se a tela de instalação de displaytone está desabilitada|
|privacyPaneDisabled|Boleano|Indica se a tela de privacidade está desabilitada|
|screenTimeScreenDisabled|Boleano|Indica se a configuração do tempo de tempo de tela está desabilitada|
|deviceNameTemplate|Cadeia de Caracteres|Define um padrão literal ou de nome.|
|configurationWebUrl|Boleano|URL para logon do assistente de instalação|

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




---
title: Tipo de recurso de depEnrollmentBaseProfile
description: O recurso DepEnrollmentBaseProfile representa um perfil de registro do Programa de Registro de Dispositivo Apple (DEP). Esse tipo de perfil deve ser atribuído aos números de série de DEP da Apple antes que os dispositivos correspondentes possam se registrar por meio de DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9b346e359922eb71fe55c9b84c6581ce2b7b0d8a
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2022
ms.locfileid: "64630684"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>Tipo de recurso de depEnrollmentBaseProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso DepEnrollmentBaseProfile representa um perfil de registro do Programa de Registro de Dispositivo Apple (DEP). Esse tipo de perfil deve ser atribuído aos números de série de DEP da Apple antes que os dispositivos correspondentes possam se registrar por meio de DEP.


Herda de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar depEnrollmentBaseProfiles](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|[Coleção de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Listar propriedades e relações dos [objetos depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .|
|[Obter depEnrollmentBaseProfile](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Leia propriedades e relações do [objeto depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O GUID do objeto Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|Nome do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|descrição|String|Descrição do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Booleano|Indica se o perfil requer autenticação de usuário Herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String|URL do ponto de extremidade de configuração a ser usada para Registro Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Booleano|Indica a autenticação com o Assistente de Instalação da Apple em vez de Portal da Empresa. Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Booleano|Indica que a Portal da Empresa é necessária em dispositivos inscritos do assistente de instalação Herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Booliano|Indica se esse é o perfil padrão|
|supervisedModeEnabled|Booliano|Modo supervisionado, True para habilitar, false caso contrário. Consulte [Registrar dispositivos no Microsoft Intune](/mem/intune/enrollment) para obter informações adicionais.|
|supportDepartment|String|Informações do departamento de suporte|
|isMandatory|Booleano|Indica se o perfil é obrigatório|
|locationDisabled|Booliano|Indica se o painel de configuração do serviço de localização está desabilitado|
|supportPhoneNumber|String|Número de telefone de suporte|
|profileRemovalDisabled|Boolean|Indica se a opção de remoção de perfil está desabilitada|
|restoreBlocked|Booliano|Indica se o painel restaurar instalação está bloqueado|
|appleIdDisabled|Booliano|Indica se o painel de configuração de ID da Apple está desabilitado|
|termsAndConditionsDisabled|Boolean|Indica se o painel de configuração 'Termos e Condições' está desabilitado|
|touchIdDisabled|Booliano|Indica se o painel de configuração de ID por toque está desabilitado|
|applePayDisabled|Booleano|Indica se o painel de configuração de pagamento da Apple está desabilitado|
|siriDisabled|Boolean|Indica se o painel de configuração de siri está desabilitado|
|diagnosticsDisabled|Boolean|Indica se o painel de configuração de diagnósticos está desabilitado|
|displayToneSetupDisabled|Booliano|Indica se a tela de instalação de displaytone está desabilitada|
|privacyPaneDisabled|Booliano|Indica se a tela de privacidade está desabilitada|
|screenTimeScreenDisabled|Boolean|Indica se a configuração do tempo de tempo de tela está desabilitada|
|deviceNameTemplate|String|Define um padrão literal ou de nome.|
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





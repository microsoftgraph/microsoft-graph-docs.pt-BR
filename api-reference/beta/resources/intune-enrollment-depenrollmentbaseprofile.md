---
title: tipo de recurso de depEnrollmentBaseProfile
description: O recurso de DepEnrollmentBaseProfile representa um perfil de inscrição do programa de inscrição de dispositivo da Apple (DEP). Esse tipo de perfil deve ser atribuído aos números de série do Apple DEP antes os dispositivos correspondentes podem registrar-se por meio do DEP.
ms.openlocfilehash: 172e0f0d4ed9b23f8c5a3d5226e24e4ac63b0527
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039924"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>tipo de recurso de depEnrollmentBaseProfile

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O recurso de DepEnrollmentBaseProfile representa um perfil de inscrição do programa de inscrição de dispositivo da Apple (DEP). Esse tipo de perfil deve ser atribuído aos números de série do Apple DEP antes os dispositivos correspondentes podem registrar-se por meio do DEP.

Herda de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista depEnrollmentBaseProfiles](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|coleção [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Lista as propriedades e os relacionamentos dos objetos [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .|
|[Obter depEnrollmentBaseProfile](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Leia as propriedades e os relacionamentos do objeto [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O GUID do objeto Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|Nome do perfil Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Descrição do perfil de Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Booliano|Indica se o perfil exige autenticação do usuário Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String|Url de ponto de extremidade de configuração a ser usado para inscrição herdada do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Booliano|Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa. Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Booliano|Indica se esse é o perfil padrão|
|supervisedModeEnabled|Booliano|Modo supervisionado, True para habilitar, false caso contrário. Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.|
|supportDepartment|String|Informações do departamento de suporte|
|passCodeDisabled|Booliano|Indica se o painel de configuração de senha está desabilitado|
|isMandatory|Booliano|Indica se o perfil é obrigatório|
|locationDisabled|Booliano|Indica se o painel de configuração do serviço local está desabilitado|
|supportPhoneNumber|String|Número de telefone de suporte|
|profileRemovalDisabled|Booliano|Indica se a opção de remoção do perfil está desabilitada|
|restoreBlocked|Booliano|Indica se o painel de configuração de restauração será bloqueado|
|appleIdDisabled|Booliano|Indica se o painel de configuração de id do Apple está desabilitado|
|termsAndConditionsDisabled|Booliano|Indica se o painel de configuração de 'Termos e condições' está desabilitado|
|touchIdDisabled|Booliano|Indica se o painel de configuração de id de toque está desabilitado|
|applePayDisabled|Booliano|Indica se o painel de configuração de pagamento do Apple está desabilitado|
|zoomDisabled|Booliano|Indica se o painel de configuração de zoom está desabilitado|
|siriDisabled|Booliano|Indica se o painel de configuração de siri está desabilitado|
|diagnosticsDisabled|Booliano|Indica se o painel de configuração de diagnósticos está desabilitado|

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
  "diagnosticsDisabled": true
}
```






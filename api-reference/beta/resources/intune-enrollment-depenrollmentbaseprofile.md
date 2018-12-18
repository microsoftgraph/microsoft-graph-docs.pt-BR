---
title: tipo de recurso de depEnrollmentBaseProfile
description: O recurso de DepEnrollmentBaseProfile representa um perfil de inscrição do programa de inscrição de dispositivo da Apple (DEP). Esse tipo de perfil deve ser atribuído aos números de série do Apple DEP antes os dispositivos correspondentes podem registrar-se por meio do DEP.
author: tfitzmac
ms.openlocfilehash: 26335fd3d35494b815dd43531ad54b4796dc861c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308369"
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
|requiresUserAuthentication|Boolean|Indica se o perfil exige autenticação do usuário Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String|Url de ponto de extremidade de configuração a ser usado para inscrição herdada do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa. Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Indica se esse é o perfil padrão|
|supervisedModeEnabled|Boolean|Modo supervisionado, True para habilitar, false caso contrário. Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.|
|supportDepartment|String|Informações do departamento de suporte|
|passCodeDisabled|Boolean|Indica se o painel de configuração de senha está desabilitado|
|isMandatory|Boolean|Indica se o perfil é obrigatório|
|locationDisabled|Boolean|Indica se o painel de configuração do serviço local está desabilitado|
|supportPhoneNumber|String|Número de telefone de suporte|
|profileRemovalDisabled|Boolean|Indica se a opção de remoção do perfil está desabilitada|
|restoreBlocked|Boolean|Indica se o painel de configuração de restauração será bloqueado|
|appleIdDisabled|Boolean|Indica se o painel de configuração de id do Apple está desabilitado|
|termsAndConditionsDisabled|Boolean|Indica se o painel de configuração de 'Termos e condições' está desabilitado|
|touchIdDisabled|Boolean|Indica se o painel de configuração de id de toque está desabilitado|
|applePayDisabled|Boolean|Indica se o painel de configuração de pagamento do Apple está desabilitado|
|zoomDisabled|Boolean|Indica se o painel de configuração de zoom está desabilitado|
|siriDisabled|Boolean|Indica se o painel de configuração de siri está desabilitado|
|diagnosticsDisabled|Boolean|Indica se o painel de configuração de diagnósticos está desabilitado|

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






---
title: Tipo de recurso depEnrollmentProfile
description: O recurso de depEnrollmentProfile representa um perfil de registro do Programa de Registro de Dispositivo Apple (DEP). Esse tipo de perfil deve ser atribuído aos números de série de DEP da Apple antes que os dispositivos correspondentes possam se registrar por meio de DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b2e6050e0807780bfc7423571fcaf51b574a0de8
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2022
ms.locfileid: "64629194"
---
# <a name="depenrollmentprofile-resource-type"></a>Tipo de recurso depEnrollmentProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso de depEnrollmentProfile representa um perfil de registro do Programa de Registro de Dispositivo Apple (DEP). Esse tipo de perfil deve ser atribuído aos números de série de DEP da Apple antes que os dispositivos correspondentes possam se registrar por meio de DEP.


Herda de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar depEnrollmentProfiles](../api/intune-enrollment-depenrollmentprofile-list.md)|[Coleção de depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Listar propriedades e relações dos [objetos depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|
|[Obter depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-get.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Leia propriedades e relações do [objeto depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|
|[Criar depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-create.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Crie um novo [objeto depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|
|[Excluir depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-delete.md)|Nenhum|Exclui um [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).|
|[Atualizar depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-update.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Atualize as propriedades de [um objeto depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|

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
|isDefault|Booliano|Indica se esse é o perfil padrão|
|supervisedModeEnabled|Booliano|Modo supervisionado, True para habilitar, false caso contrário. Consulte [Registrar dispositivos no Microsoft Intune](/mem/intune/enrollment) para obter informações adicionais.|
|supportDepartment|String|Informações do departamento de suporte|
|passCodeDisabled|Boolean|Indica se o painel de configuração senha está desabilitado|
|isMandatory|Booliano|Indica se o perfil é obrigatório|
|locationDisabled|Boolean|Indica se o painel de configuração do serviço de localização está desabilitado|
|supportPhoneNumber|String|Número de telefone de suporte|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|Indica o modo de emparelhamento do iTunes. Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.|
|profileRemovalDisabled|Booleano|Indica se a opção de remoção de perfil está desabilitada|
|managementCertificates|[coleção managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)|Certificados de gerenciamento para o Apple Configurator|
|restoreBlocked|Booliano|Indica se o painel restaurar instalação está bloqueado|
|restoreFromAndroidDisabled|Booleano|Indica se a restauração do Android está desabilitada|
|appleIdDisabled|Booleano|Indica se o painel de configuração de ID da Apple está desabilitado|
|termsAndConditionsDisabled|Boolean|Indica se o painel de configuração 'Termos e Condições' está desabilitado|
|touchIdDisabled|Boolean|Indica se o painel de configuração de ID por toque está desabilitado|
|applePayDisabled|Booliano|Indica se o painel de configuração de pagamento da Apple está desabilitado|
|zoomDisabled|Booliano|Indica se o painel de configuração de zoom está desabilitado|
|siriDisabled|Booliano|Indica se o painel de configuração de siri está desabilitado|
|diagnosticsDisabled|Booliano|Indica se o painel de configuração de diagnósticos está desabilitado|
|macOSRegistrationDisabled|Boolean|Indica se o registro do Mac OS está desabilitado|
|macOSFileVaultDisabled|Booleano|Indica se o cofre de arquivos do Mac OS está desabilitado|
|awaitDeviceConfiguredConfirmation|Booliano|Indica se o dispositivo precisará aguardar a confirmação configurada|
|sharedIPadMaximumUserCount|Int32|Isso especifica o número máximo de usuários que podem usar um iPad. Aplicável somente no modo iPad compartilhado.|
|enableSharedIPad|Booliano|Isso indica se o dispositivo deve ser inscrito em um modo que habilita cenários de vários usuários. Aplicável somente em iPads compartilhados.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
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
  "iTunesPairingMode": "String",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true
}
```





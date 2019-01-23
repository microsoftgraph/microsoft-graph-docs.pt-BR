---
title: tipo de recurso de depEnrollmentProfile
description: O recurso de depEnrollmentProfile representa um perfil de inscrição do programa de inscrição de dispositivo da Apple (DEP). Esse tipo de perfil deve ser atribuído aos números de série do Apple DEP antes os dispositivos correspondentes podem registrar-se por meio do DEP.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 61119a97deb41807e6eee66f0ef3376035500190
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395899"
---
# <a name="depenrollmentprofile-resource-type"></a>tipo de recurso de depEnrollmentProfile

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

O recurso de depEnrollmentProfile representa um perfil de inscrição do programa de inscrição de dispositivo da Apple (DEP). Esse tipo de perfil deve ser atribuído aos números de série do Apple DEP antes os dispositivos correspondentes podem registrar-se por meio do DEP.


Herda de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista depEnrollmentProfiles](../api/intune-enrollment-depenrollmentprofile-list.md)|coleção [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Lista as propriedades e os relacionamentos dos objetos [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|
|[Obter depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-get.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Leia as propriedades e os relacionamentos do objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|
|[Criar depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-create.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Crie um novo objeto de [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|
|[Excluir depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-delete.md)|Nenhum|Exclui um [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).|
|[Atualizar depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-update.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Atualize as propriedades de um objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O GUID do objeto Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|Nome do perfil Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Descrição do perfil de Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boolean|Indica se o perfil exige autenticação do usuário Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String|Url de ponto de extremidade de configuração a ser usado para inscrição herdada do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa. Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|Indica que o Portal da empresa é necessária em dispositivos de inscritos do Assistente de instalação Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Indica se esse é o perfil padrão|
|supervisedModeEnabled|Boolean|Modo supervisionado, True para habilitar, false caso contrário. Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.|
|supportDepartment|String|Informações do departamento de suporte|
|passCodeDisabled|Boolean|Indica se o painel de configuração de senha está desabilitado|
|isMandatory|Boolean|Indica se o perfil é obrigatório|
|locationDisabled|Boolean|Indica se o painel de configuração do serviço local está desabilitado|
|supportPhoneNumber|String|Número de telefone de suporte|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|Indica a modo de emparelhamento de iTunes. Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.|
|profileRemovalDisabled|Boolean|Indica se a opção de remoção do perfil está desabilitada|
|managementCertificates|coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)|Certificados de gerenciamento para configurador da Apple|
|restoreBlocked|Boolean|Indica se o painel de configuração de restauração será bloqueado|
|restoreFromAndroidDisabled|Boolean|Indica se a restauração do Android está desabilitada|
|appleIdDisabled|Boolean|Indica se o painel de configuração de id do Apple está desabilitado|
|termsAndConditionsDisabled|Boolean|Indica se o painel de configuração de 'Termos e condições' está desabilitado|
|touchIdDisabled|Boolean|Indica se o painel de configuração de id de toque está desabilitado|
|applePayDisabled|Boolean|Indica se o painel de configuração de pagamento do Apple está desabilitado|
|zoomDisabled|Boolean|Indica se o painel de configuração de zoom está desabilitado|
|siriDisabled|Boolean|Indica se o painel de configuração de siri está desabilitado|
|diagnosticsDisabled|Boolean|Indica se o painel de configuração de diagnósticos está desabilitado|
|macOSRegistrationDisabled|Boolean|Indica se o registro do Mac OS está desabilitado|
|macOSFileVaultDisabled|Boolean|Indica se o armazenamento de arquivo do Mac OS está desabilitado|
|awaitDeviceConfiguredConfirmation|Boolean|Indica se o dispositivo será necessário aguardar a confirmação configurada|
|sharedIPadMaximumUserCount|Int32|Especifica o número máximo de usuários que podem utilizar um iPad compartilhado. Só é aplicável no modo compartilhado iPad.|
|enableSharedIPad|Boolean|Isso indica se o dispositivo é registrado em um modo que permite que vários cenários de usuário. Só é aplicável no compartilhados iPads.|

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





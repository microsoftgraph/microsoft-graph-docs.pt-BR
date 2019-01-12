---
title: tipo de recurso de enrollmentProfile
description: O recurso de enrollmentProfile representa uma coleção de configurações que devem ser fornecidas a inscrição prévia para habilitar inscrevendo determinados dispositivos cujas identidades foram pré-configurados. As identidades de dispositivo pré-configurados são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: b88745c060e71e32199a96b23f94fa0d3229d451
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935588"
---
# <a name="enrollmentprofile-resource-type"></a>tipo de recurso de enrollmentProfile

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O recurso de enrollmentProfile representa uma coleção de configurações que devem ser fornecidas a inscrição prévia para habilitar inscrevendo determinados dispositivos cujas identidades foram pré-configurados. As identidades de dispositivo pré-configurados são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista enrollmentProfiles](../api/intune-enrollment-enrollmentprofile-list.md)|coleção [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Lista as propriedades e os relacionamentos dos objetos [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[Obter enrollmentProfile](../api/intune-enrollment-enrollmentprofile-get.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Leia as propriedades e os relacionamentos do objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[Criar enrollmentProfile](../api/intune-enrollment-enrollmentprofile-create.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Crie um novo objeto de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[Excluir enrollmentProfile](../api/intune-enrollment-enrollmentprofile-delete.md)|Nenhum|Exclui um [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).|
|[Atualizar enrollmentProfile](../api/intune-enrollment-enrollmentprofile-update.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Atualize as propriedades de um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[ação de setDefaultProfile](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|Nenhum|Ainda não documentado|
|[função exportMobileConfig](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|Cadeia de caracteres|Exporta a configuração móvel|
|[ação de updateDeviceProfileAssignment](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto.|
|displayName|Cadeia de caracteres|Nome do perfil|
|description|Cadeia de caracteres|Descrição do perfil|
|requiresUserAuthentication|Booliano|Indica se o perfil exige autenticação do usuário|
|configurationEndpointUrl|Cadeia de caracteres|Url de ponto de extremidade de configuração a ser usado para registro|
|enableAuthenticationViaCompanyPortal|Booliano|Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true
}
```






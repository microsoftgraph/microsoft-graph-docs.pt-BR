---
title: Tipo de recurso enrollmentProfile
description: O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas antes do registro para habilitar o registro de determinados dispositivos cujas identidades foram pré-em estágios. As identidades de dispositivo pré-em estágios são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bae158fb33e4d1fccc4e5b4b6fd527b0d17cc9df
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59141085"
---
# <a name="enrollmentprofile-resource-type"></a>Tipo de recurso enrollmentProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas antes do registro para habilitar o registro de determinados dispositivos cujas identidades foram pré-em estágios. As identidades de dispositivo pré-em estágios são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar enrollmentProfiles](../api/intune-enrollment-enrollmentprofile-list.md)|[Coleção enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Listar propriedades e relações dos objetos [enrollmentProfile.](../resources/intune-enrollment-enrollmentprofile.md)|
|[Obter enrollmentProfile](../api/intune-enrollment-enrollmentprofile-get.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Ler propriedades e relações do [objeto enrollmentProfile.](../resources/intune-enrollment-enrollmentprofile.md)|
|[Criar enrollmentProfile](../api/intune-enrollment-enrollmentprofile-create.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Crie um novo [objeto enrollmentProfile.](../resources/intune-enrollment-enrollmentprofile.md)|
|[Excluir enrollmentProfile](../api/intune-enrollment-enrollmentprofile-delete.md)|Nenhum|Exclui um [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).|
|[Atualizar enrollmentProfile](../api/intune-enrollment-enrollmentprofile-update.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Atualize as propriedades de [um objeto enrollmentProfile.](../resources/intune-enrollment-enrollmentprofile.md)|
|[Ação setDefaultProfile](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|Nenhuma|Ainda não documentado|
|[Função exportMobileConfig](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|Cadeia de Caracteres|Exporta a configuração móvel|
|[Ação updateDeviceProfileAssignment](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto.|
|displayName|Cadeia de caracteres|Nome do perfil|
|description|Cadeia de caracteres|Descrição do perfil|
|requiresUserAuthentication|Boleano|Indica se o perfil requer autenticação do usuário|
|configurationEndpointUrl|Cadeia de Caracteres|URL do ponto de extremidade de configuração a ser usada para Registro|
|enableAuthenticationViaCompanyPortal|Boleano|Indica a autenticação com o Assistente de Instalação da Apple em vez de Portal da Empresa.|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boleano|Indica que a Portal da Empresa é necessária em dispositivos inscritos pelo assistente de instalação|

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
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```




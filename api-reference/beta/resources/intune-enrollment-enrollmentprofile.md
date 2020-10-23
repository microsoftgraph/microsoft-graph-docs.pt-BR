---
title: tipo de recurso enrollmentProfile
description: O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas como pré-registro para habilitar a inscrição de determinados dispositivos cujas identidades foram pré-configuradas. As identidades de dispositivo pré-configuradas são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0c8837bdcc87abc3866441c4c81dee163dcf13bb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707749"
---
# <a name="enrollmentprofile-resource-type"></a>tipo de recurso enrollmentProfile

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas como pré-registro para habilitar a inscrição de determinados dispositivos cujas identidades foram pré-configuradas. As identidades de dispositivo pré-configuradas são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar enrollmentProfiles](../api/intune-enrollment-enrollmentprofile-list.md)|coleção [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Listar Propriedades e relações dos objetos [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[Obter enrollmentProfile](../api/intune-enrollment-enrollmentprofile-get.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Leia as propriedades e as relações do objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[Criar enrollmentProfile](../api/intune-enrollment-enrollmentprofile-create.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Criar um novo objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[Excluir enrollmentProfile](../api/intune-enrollment-enrollmentprofile-delete.md)|Nenhum|Exclui [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).|
|[Atualizar enrollmentProfile](../api/intune-enrollment-enrollmentprofile-update.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Atualiza as propriedades de um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[Ação setDefaultProfile](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|Nenhuma|Ainda não documentado|
|[função função exportmobileconfig](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|String|Exporta a configuração móvel|
|[Ação updateDeviceProfileAssignment](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O GUID do objeto.|
|displayName|String|Nome do perfil|
|description|String|Descrição do perfil|
|requiresUserAuthentication|Boolean|Indica se o perfil requer autenticação do usuário|
|configurationEndpointUrl|String|URL de ponto de extremidade de configuração a ser usada para registro|
|Enableauthenticationviacompanyportal foi adicionada|Boolean|Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados|

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






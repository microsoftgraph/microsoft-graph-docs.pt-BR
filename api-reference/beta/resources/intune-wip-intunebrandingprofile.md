---
title: tipo de recurso intuneBrandingProfile
description: Esta entidade contém dados que são usados na personalização da aparência do nível do locatário dos aplicativos do portal da empresa, bem como do portal da Web do usuário final.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6063b07ed9361b00315a7c8a2b170cea72f7dff3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371905"
---
# <a name="intunebrandingprofile-resource-type"></a>tipo de recurso intuneBrandingProfile

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Esta entidade contém dados que são usados na personalização da aparência do nível do locatário dos aplicativos do portal da empresa, bem como do portal da Web do usuário final.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar Navegaçãointunebrandingprofiles](../api/intune-wip-intunebrandingprofile-list.md)|coleção [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Listar Propriedades e relações dos objetos [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|
|[Obter intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Leia as propriedades e as relações do objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|
|[Criar intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Criar um novo objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|
|[Excluir intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-delete.md)|Nenhum|Exclui [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).|
|[Atualizar intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Atualiza as propriedades de um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|
|[atribuir ação](../api/intune-wip-intunebrandingprofile-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave de perfil|
|ProfileName|String|Nome do perfil|
|profileDescription|String|Descrição do perfil|
|isDefaultProfile|Booliano|Booliano que indica se o perfil é usado como padrão ou não|
|createdDateTime|DateTimeOffset|Hora em que o BrandingProfile foi criado|
|lastModifiedDateTime|DateTimeOffset|Hora em que a BrandingProfile foi modificada pela última vez|
|displayName|String|Nome da empresa/organização que é exibido para os usuários finais|
|contactITName|String|Nome da pessoa/organização responsável pelo suporte de ti|
|contactITPhoneNumber|String|Número de telefone da pessoa/organização responsável pelo suporte de ti|
|contactITEmailAddress|String|Endereço de email da pessoa/organização responsável pelo suporte de ti|
|contactITNotes|String|Comentários de texto sobre a pessoa/organização responsável pelo suporte de ti|
|privacyUrl|String|URL para a política de privacidade da empresa/organização|
|onlineSupportSiteUrl|String|URL para o site de assistência técnica de ti da empresa/organização|
|onlineSupportSiteName|Cadeia de caracteres|Nome para exibição do site de assistência técnica de ti da empresa/organização|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Cor do tema principal usada nos aplicativos do portal da empresa e no portal da Web|
|showLogo|Booliano|Booliano que indica se as imagens de logotipo fornecidas pelo administrador são mostradas ou não|
|showDisplayNameNextToLogo|Booliano|Booliano que indica se o nome de exibição fornecido pelo administrador será mostrado ao lado da imagem de logotipo ou não|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo de cor de tema atrás do logotipo|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo claro atrás do logotipo|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem personalizada exibida na página inicial dos aplicativos do portal da empresa|
|customPrivacyMessage|String|Comentários de texto sobre o que o administrador tem acesso ao no dispositivo|
|isRemoveDeviceDisabled|Booliano|Booliano que indica se o adminsistrator desabilitou a ação "remover dispositivo" em dispositivos corporativos de propriedade.|
|isFactoryResetDisabled|Booliano|Booliano que indica se o adminsistrator desabilitou a ação "redefinição de fábrica" em dispositivos corporativos de propriedade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|A lista de atribuições de grupo para o perfil de identidade visual|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrandingProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "String (identifier)",
  "profileName": "String",
  "profileDescription": "String",
  "isDefaultProfile": true,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "customPrivacyMessage": "String",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true
}
```




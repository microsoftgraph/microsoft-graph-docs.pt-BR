---
title: tipo de recurso intuneBrandingProfile
description: Esta entidade contém dados que são usados na personalização da aparência do nível do locatário dos aplicativos do portal da empresa, bem como do portal da Web do usuário final.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f21cc97cd701f9826743475c4055aed6bafe9ca
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144699"
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
|[Ação assign](../api/intune-wip-intunebrandingprofile-assign.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave de perfil|
|ProfileName|String|Nome do perfil|
|profileDescription|String|Descrição do perfil|
|isDefaultProfile|Booliano|Apresenta se o perfil é usado para o padrão.|
|createdDateTime|DateTimeOffset|Quando o BrandingProfile foi criado.|
|lastModifiedDateTime|DateTimeOffset|Quando o BrandingProfile foi modificado pela última vez.|
|displayName|String|Nome da empresa/organização exibido para usuários finais.|
|contactITName|String|Nome da pessoa/organização responsável pelo suporte de TI.|
|contactITPhoneNumber|String|Número de telefone da pessoa/organização responsável pelo suporte de TI.|
|contactITEmailAddress|String|Endereço de email da pessoa/organização responsável pelo suporte de TI.|
|contactITNotes|String|Comentários de texto relacionados à pessoa/organização responsável pelo suporte de TI.|
|privacyUrl|String|URL da política de privacidade da empresa/organização.|
|onlineSupportSiteUrl|String|URL do site de assistência técnica de TI da empresa/organização.|
|onlineSupportSiteName|Cadeia de caracteres|Nome de exibição do site de assistência técnica de TI da empresa/organização.|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Cor de tema principal usado nos aplicativos e no portal da Web do Portal da Empresa.|
|showLogo|Booliano|Booliano que indica se as imagens de logotipo fornecidas pelo administrador serão exibidas ou não.|
|showDisplayNameNextToLogo|Booliano|Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem do logotipo exibida nos aplicativos do portal da empresa em planos de fundo de cores de tema.|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem do logotipo exibida nos aplicativos do portal da empresa em planos de fundo claros.|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem personalizada exibida na página inicial dos aplicativos do portal da empresa|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|A lista de atribuições de grupo para o perfil de identidade visual.|

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
  }
}
```





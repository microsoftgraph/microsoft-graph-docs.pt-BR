---
title: tipo de recurso de intuneBrandingProfile
description: Essa entidade contém dados que são utilizados em Personalizar a aparência de nível de locatário de aplicativos do Portal da empresa, bem como o portal da web de usuário final.
ms.openlocfilehash: b85f33731f91a5b239a00a2a537f5e0fdbef56a9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033490"
---
# <a name="intunebrandingprofile-resource-type"></a>tipo de recurso de intuneBrandingProfile

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Essa entidade contém dados que são utilizados em Personalizar a aparência de nível de locatário de aplicativos do Portal da empresa, bem como o portal da web de usuário final.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista intuneBrandingProfiles](../api/intune-wip-intunebrandingprofile-list.md)|coleção [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Lista as propriedades e os relacionamentos dos objetos [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|
|[Obter intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Leia as propriedades e os relacionamentos do objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|
|[Criar intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Crie um novo objeto de [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|
|[Excluir intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-delete.md)|Nenhum|Exclui um [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).|
|[Atualizar intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Atualize as propriedades de um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave de perfil|
|profileName|String|Nome do perfil|
|profileDescription|String|Descrição do perfil|
|isDefaultProfile|Booliano|Apresenta se o perfil é usado para padrão.|
|createdDateTime|DateTimeOffset|Quando o BrandingProfile foi criado.|
|lastModifiedDateTime|DateTimeOffset|Quando o BrandingProfile última modificação.|
|displayName|Cadeia de caracteres|Nome da empresa/organização exibido para usuários finais.|
|contactITName|Cadeia de caracteres|Nome da pessoa/organização responsável pelo suporte de TI.|
|contactITPhoneNumber|Cadeia de caracteres|Número de telefone da pessoa/organização responsável pelo suporte de TI.|
|contactITEmailAddress|Cadeia de caracteres|Endereço de email da pessoa/organização responsável pelo suporte de TI.|
|contactITNotes|Cadeia de caracteres|Comentários de texto relacionados à pessoa/organização responsável pelo suporte de TI.|
|privacyUrl|Cadeia de caracteres|URL da política de privacidade da empresa/organização.|
|onlineSupportSiteUrl|Cadeia de caracteres|URL do site de assistência técnica de TI da empresa/organização.|
|onlineSupportSiteName|Cadeia de caracteres|Nome de exibição do site de assistência técnica de TI da empresa/organização.|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Cor de tema principal usado nos aplicativos e no portal da Web do Portal da Empresa.|
|showLogo|Booliano|Booliano que indica se as imagens de logotipo fornecidas pelo administrador serão exibidas ou não.|
|showDisplayNameNextToLogo|Booliano|Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem de logotipo exibida nos aplicativos de Portal da empresa nos planos de fundo de cores de tema.|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem de logotipo exibida nos aplicativos de Portal da empresa nos planos de fundo claras.|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem personalizada exibida na página inicial de aplicativos de Portal da empresa|

## <a name="relationships"></a>Relações
Nenhum
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






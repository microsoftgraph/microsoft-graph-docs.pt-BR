---
title: Tipo de recurso intuneBrand
description: intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.
ms.openlocfilehash: b8ed558e2be032110470cc4e2c64d27d8011af1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038846"
---
# <a name="intunebrand-resource-type"></a>Tipo de recurso intuneBrand

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
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
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem do logotipo exibida nos aplicativos do Portal da Empresa que têm um plano de fundo claro atrás do logotipo.|
|darkBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem do logotipo exibida nos aplicativos do Portal da Empresa que têm um plano de fundo escuro atrás do logotipo.|
|showNameNextToLogo|Booliano|Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem personalizada exibida na página inicial do Portal de Compnay app|
|showDisplayNameNextToLogo|Booliano|Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
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
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showNameNextToLogo": true,
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showDisplayNameNextToLogo": true
}
```






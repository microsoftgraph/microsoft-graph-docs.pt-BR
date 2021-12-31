---
title: Tipo de recurso organizationalBrandingProperties
description: Contém detalhes da identidade visual da organização.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ea267c224bf8e7d67f439029a5648861154b9463
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61646925"
---
# <a name="organizationalbrandingproperties-resource-type"></a>Tipo de recurso organizationalBrandingProperties

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo abstrato que expõe propriedades para configurar a identidade visual de uma organização.

As organizações podem personalizar as páginas de Azure Active Directory (Azure AD) que aparecem quando os usuários entrarem nos aplicativos específicos do locatário da organização ou quando o Azure AD identificar o locatário do usuário do nome de usuário. Um desenvolvedor também pode ler as informações de identidade visual da empresa e personalizar sua experiência de aplicativo para adaptá-la especificamente para o usuário que está assinado usando a identidade visual da empresa.

Não é possível alterar o idioma da configuração original como representado pelo [objeto organizationalBranding.](organizationalbranding.md) No entanto, as empresas podem adicionar identidade visual diferente com base na localidade. Para identidade visual específica do idioma, consulte o [objeto organizationalBrandingLocalization.](organizationalbrandinglocalization.md)

>[!NOTE]
>A adição de identidade visual personalizada exige que você tenha licenças Azure Active Directory (Azure AD) Premium 1, Premium 2 ou Office 365 (para aplicativos Office 365). Para obter mais informações sobre licenciamento e edições, consulte [Inscrever-se Azure AD Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium).
>
>Azure AD Premium edições estão disponíveis para clientes na China usando a instância mundial de Azure Active Directory. Azure AD Premium edições não têm suporte no serviço do Azure operado pela 21Vianet na China. Para obter mais informações, fale conosco usando o [fórum Azure Active Directory fórum](https://feedback.azure.com/forums/169401-azure-active-directory/).

## <a name="methods"></a>Métodos
Nenhum.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| backgroundColor | String | Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda. Recomendamos que você use a cor primária do logotipo da faixa ou da cor da sua organização. Especifique isso no formato hexadecimal, por exemplo, branco é `#FFFFFF` . |
| backgroundImage | Stream | Imagem que aparece como o plano de fundo da página de login. Os tipos permitidos são PNG ou JPEG não menores que 300 KB e não maiores que 1920 × 1080 pixels. Uma imagem menor reduzirá os requisitos de largura de banda e tornará a carga da página mais rápida. |
| backgroundImageRelativeUrl | String | Uma URL relativa para a **propriedade backgroundImage** combinada com uma URL base CDN **cdnList** para fornecer a versão atendida por um CDN. Somente leitura. |
| bannerLogo | Stream | Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada. Os tipos permitidos são PNG ou JPEG não maiores que 36 × 245 pixels. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo. |
| bannerLogoRelativeUrl | String | Uma URL relativa para a **propriedade bannerLogo** que é combinada com uma URL base CDN **da cdnList** para fornecer a versão somente leitura atendida por um CDN. Somente leitura. |
| cdnList | Coleção String | Uma lista de URLs base para todos os provedores CDN disponíveis que estão servindo os ativos do recurso atual. Vários CDN provedores são usados ao mesmo tempo para alta disponibilidade de solicitações de leitura. Somente leitura. |
| id | String | Um identificador que representa a localidade especificada usando nomes de cultura. Os nomes de cultura seguem o padrão RFC 1766 no formato "languagecode2-country/regioncode2", onde "languagecode2" é um código de duas letras minúsculo derivado da ISO 639-1 e "country/regioncode2" é um código de duas letras maiúscula derivado da ISO 3166. Por exemplo, inglês dos EUA é `en-US` . A **id para** o padrão /branding é sempre os tipos de cadeia de caracteres `0` ou `default` . Somente leitura. <br/><br/>**OBSERVAÇÃO:** No momento, não há suporte para várias marcas para uma única localidade. |
| signInPageText | String | Texto que aparece na parte inferior da caixa de login. Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal. Este texto deve ser Unicode e não exceder 1024 caracteres. |
| squareLogo | Stream | Uma versão quadrada do logotipo da sua empresa que aparece Windows 10 experiências in-loco (OOBE) e quando o Windows Autopilot está habilitado para implantação. Os tipos permitidos são PNG ou JPEG não maiores que 240 x 240 pixels e no máximo 10 KB de tamanho. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo. |
| squareLogoRelativeUrl | String | Uma URL relativa para a **propriedade squareLogo** que é combinada com uma URL base CDN **da cdnList** para fornecer a versão atendida por um CDN. Somente leitura. |
| usernameHintText | String | Cadeia de caracteres que mostra como a dica na caixa de texto do nome de usuário na tela de entrada. Este texto deve ser um Unicode, sem links ou código, e não pode exceder 64 caracteres. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organizationalBrandingProperties",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organizationalBrandingProperties",
  "id": "String (identifier)",
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "backgroundImageRelativeUrl": "String",
  "bannerLogo": "Stream",
  "bannerLogoRelativeUrl": "String",
  "cdnList": [
    "String"
  ],
  "signInPageText": "String",
  "squareLogo": "Stream",
  "squareLogoRelativeUrl": "String",
  "usernameHintText": "String"
}
```


---
title: Tipo de recurso organizationalBrandingProperties
description: Contém detalhes da identidade visual da organização.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 68831b6069df0ea94df36605ff9f1099dfd27feb
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2022
ms.locfileid: "62805141"
---
# <a name="organizationalbrandingproperties-resource-type"></a>Tipo de recurso organizationalBrandingProperties

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo abstrato que expõe propriedades para configurar a identidade visual de uma organização.

As organizações podem personalizar as páginas de Azure Active Directory (Azure AD) que aparecem quando os usuários entrarem nos aplicativos específicos do locatário da organização ou quando o Azure AD identificar o locatário do usuário do nome de usuário. Um desenvolvedor também pode ler as informações de identidade visual da empresa e personalizar sua experiência de aplicativo para adaptá-la especificamente para o usuário que está assinado usando a identidade visual da empresa.

Não é possível alterar o idioma da configuração original como representado pelo [objeto organizationalBranding](organizationalbranding.md) . No entanto, as empresas podem adicionar identidade visual diferente com base na localidade. Para identidade visual específica do idioma, consulte o [objeto organizationalBrandingLocalization](organizationalbrandinglocalization.md) .

>[!NOTE]
>A adição de identidade visual personalizada exige que você tenha licenças Azure Active Directory (Azure AD) Premium 1, Premium 2 ou Office 365 (para aplicativos Office 365). Para obter mais informações sobre licenciamento e edições, consulte [Inscrever-se Azure AD Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium).
>
>Azure AD Premium edições estão disponíveis para clientes na China usando a instância mundial de Azure Active Directory. Azure AD Premium edições não têm suporte no serviço do Azure operado pela 21Vianet na China. Para obter mais informações, fale conosco usando o [fórum Azure Active Directory fórum](https://feedback.azure.com/forums/169401-azure-active-directory/).

## <a name="methods"></a>Métodos
Nenhum.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| backgroundColor | Cadeia de caracteres | Cor que aparece no lugar da imagem de plano de fundo em conexões de baixa largura de banda. Recomendamos que você use a cor primária do logotipo da faixa ou da cor da sua organização. Especifique isso no formato hexadecimal, por exemplo, branco é `#FFFFFF`. |
| backgroundImage | Stream | Imagem que aparece como o plano de fundo da página de login. Os tipos permitidos são PNG ou JPEG não menores que 300 KB e não maiores que 1920 × 1080 pixels. Uma imagem menor reduzirá os requisitos de largura de banda e tornará a carga da página mais rápida. |
| backgroundImageRelativeUrl | Cadeia de caracteres | Uma URL relativa para a **propriedade backgroundImage** combinada com uma URL base CDN **cdnList** para fornecer a versão atendida por um CDN. Somente leitura. |
| bannerLogo | Stream | Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada. Os tipos permitidos são PNG ou JPEG não maiores que 36 × 245 pixels. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo. |
| bannerLogoRelativeUrl | Cadeia de caracteres | Uma URL relativa para a **propriedade bannerLogo** combinada com uma URL base CDN **cdnList** para fornecer a versão somente leitura atendida por um CDN. Somente leitura. |
| cdnList | String collection | Uma lista de URLs base para todos os provedores CDN disponíveis que estão servindo os ativos do recurso atual. Vários CDN provedores são usados ao mesmo tempo para alta disponibilidade de solicitações de leitura. Somente leitura. |
| customAccountResetCredentialsUrl | Cadeia de caracteres | Uma URL personalizada para redefinir credenciais de conta. Essa URL deve estar no formato ASCII ou caracteres não ASCII devem ser codificados em URL e não exceder 128 caracteres. |
| customCannotAccessYourAccountText | Cadeia de caracteres | Uma cadeia de caracteres para substituir o padrão "Não é possível acessar sua conta?" texto de hiperlink de redefinição de senha de autoatendados (SSPR) na página de login. Este texto deve estar no formato Unicode e não exceder 256 caracteres. |
| customCannotAccessYourAccountUrl | Cadeia de caracteres | Uma URL personalizada para substituir a URL padrão da redefinição de senha de autoatendência (SSPR) "Não é possível acessar sua conta?" hiperlink na página de login. Essa URL deve estar no formato ASCII ou caracteres não ASCII devem ser codificados em URL e não exceder 128 caracteres. <br/><br/>**NÃO USE.** Use **customAccountResetCredentialsUrl** . |
| customForgotMyPasswordText | Cadeia de caracteres | Uma cadeia de caracteres para substituir o texto padrão do hiperlink "Esqueci minha senha" no formulário de login. Este texto deve estar no formato Unicode e não exceder 256 caracteres. |
| customPrivacyAndCookiesText | Cadeia de caracteres | Uma cadeia de caracteres para substituir o texto padrão de hiperlink "Privacidade e Cookies" no rodapé. Este texto deve estar no formato Unicode e não exceder 256 caracteres. |
| customPrivacyAndCookiesUrl | Cadeia de caracteres | Uma URL personalizada para substituir a URL padrão do hiperlink "Privacidade e Cookies" no rodapé. Essa URL deve estar no formato ASCII ou caracteres não ASCII devem ser codificados em URL e não exceder 128 caracteres. |
| customResetItNowText | Cadeia de caracteres | Uma cadeia de caracteres para substituir o texto padrão do hiperlink "redefini-lo agora" no formulário de login. Este texto deve estar no formato Unicode e não exceder 256 caracteres. <br/><br/>**NÃO USE:** No momento, não há suporte para personalização do texto do hiperlink "redefini-lo agora". |
| customTermsOfUseText | Cadeia de caracteres | Uma cadeia de caracteres para substituir o texto padrão de hiperlink "Termos de Uso" no rodapé. Este texto deve estar no formato Unicode e não exceder 256 caracteres. |
| customTermsOfUseUrl | Cadeia de caracteres | Uma URL personalizada para substituir a URL padrão do hiperlink "Termos de Uso" no rodapé. Essa URL deve estar no formato ASCII ou caracteres não ASCII devem ser codificados por URL e não exceder 128characters. |
| favicon | Stream | Um ícone personalizado (favicon) para substituir um favicon de produto padrão da Microsoft em um locatário do Azure AD. |
| faviconRelativeUrl | Cadeia de caracteres | Uma URL relativa para o favicon acima que é combinada com uma URL CDN base da **cdnList** para fornecer a versão atendida por um CDN. Somente leitura. |
| headerBackgroundColor | Cadeia de caracteres | A cor RGB a ser aplicada para personalizar a cor do header. |
| id | Cadeia de caracteres | Um identificador que representa a localidade especificada usando nomes de cultura. Os nomes de cultura seguem o padrão RFC 1766 no formato "languagecode2-country/regioncode2", onde "languagecode2" é um código de duas letras minúsculo derivado da ISO 639-1 e "country/regioncode2" é um código de duas letras maiúscula derivado da ISO 3166. Por exemplo, inglês dos EUA é `en-US`. A **id para** o padrão /branding é sempre os tipos de cadeia de caracteres `0` ou `default`. Somente leitura. <br/><br/>**OBSERVAÇÃO:** No momento, não há suporte para várias marcas para uma única localidade. |
| loginPageTextVisibilitySettings | [loginPageTextVisibilitySettings](loginPageTextVisibilitySettings.md) | Representa os vários textos que podem ser ocultos na página de logon de um locatário. |
| signInPageText | Cadeia de caracteres | Texto que aparece na parte inferior da caixa de login. Use isso para comunicar informações adicionais, como o número de telefone para sua assistência médica ou uma declaração legal. Este texto deve estar no formato Unicode e não exceder 1024 caracteres. |
| squareLogo | Stream | Uma versão quadrada do logotipo da sua empresa que aparece Windows 10 experiências in-loco (OOBE) e quando o Windows Autopilot está habilitado para implantação. Os tipos permitidos são PNG ou JPEG não maiores que 240 x 240 pixels e não mais de 10 KB de tamanho. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.|
| squareLogoRelativeUrl | Cadeia de caracteres | Uma URL relativa para a **propriedade squareLogo** combinada com uma URL base CDN **cdnList** para fornecer a versão atendida por um CDN. Somente leitura. |
| usernameHintText | Cadeia de caracteres | Uma cadeia de caracteres que mostra como a dica na caixa de texto do nome de usuário na tela de entrada. Este texto deve ser um Unicode, sem links ou código, e não pode exceder 64 caracteres. |

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
  "usernameHintText": "String",
  "customAccountResetCredentialsUrl": "String",
  "customCannotAccessYourAccountText": "String",
  "customCannotAccessYourAccountUrl": "String",
  "customForgotMyPasswordText": "String",
  "customPrivacyAndCookiesText": "String",
  "customPrivacyAndCookiesUrl": "String",
  "customResetItNowText": "String",
  "customTermsOfUseText": "String",
  "customTermsOfUseUrl": "String",
  "favicon": "Stream",
  "faviconRelativeUrl": "String",
  "headerBackgroundColor": "String",
  "loginPageTextVisibilitySettings": {
    "@odata.type": "microsoft.graph.loginPageTextVisibilitySettings"
  }
}
```

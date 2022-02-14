---
title: Tipo de recurso organizationalBrandingLocalization
description: Contém detalhes das localizações de identidade visual da organização.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b01a52bd81c5b1cbbaf8611ab0efd96c75f229b5
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804622"
---
# <a name="organizationalbrandinglocalization-resource-type"></a>Tipo de recurso organizationalBrandingLocalization

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recurso que oferece suporte ao gerenciamento de identidade visual específica do idioma. Embora você não possa alterar o idioma da configuração original, esse recurso permite que você crie uma nova configuração para um idioma diferente.

Herda de [organizationalBrandingProperties](organizationalbrandingproperties.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar organizationalBrandingLocalizations](../api/organizationalbranding-list-localizations.md)|coleção [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Obter uma lista dos objetos [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) e suas propriedades.|
|[Criar organizationalBrandingLocalization](../api/organizationalbranding-post-localizations.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Crie um novo [objeto organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) .|
|[Obter organizationalBrandingLocalization](../api/organizationalbrandinglocalization-get.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Leia as propriedades e as relações de um [objeto organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) .|
|[Atualizar organizationalBrandingLocalization](../api/organizationalbrandinglocalization-update.md)| Nenhum |Atualize as propriedades de um [objeto organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) .|
|[Excluir organizationalBrandingLocalization](../api/organizationalbrandinglocalization-delete.md)|Nenhum|Exclui um [objeto organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) .|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| backgroundColor | Cadeia de caracteres | Cor que aparece no lugar da imagem de plano de fundo em conexões de baixa largura de banda. Recomendamos que você use a cor primária do logotipo da faixa ou da cor da sua organização. Especifique isso no formato hexadecimal, por exemplo, branco é `#FFFFFF`. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| backgroundImage | Stream | Imagem que aparece como o plano de fundo da página de login. Os tipos permitidos são PNG ou JPEG não menores que 300 KB e não maiores que 1920 × 1080 pixels. Uma imagem menor reduzirá os requisitos de largura de banda e tornará a carga da página mais rápida. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| backgroundImageRelativeUrl | Cadeia de caracteres | Uma URL relativa para a **propriedade backgroundImage** combinada com uma URL base CDN **cdnList** para fornecer a versão atendida por um CDN. Somente leitura. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| bannerLogo | Stream | Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada. Os tipos permitidos são PNG ou JPEG não maiores que 36 × 245 pixels. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| bannerLogoRelativeUrl | Cadeia de caracteres | Uma URL relativa para a **propriedade bannerLogo** combinada com uma URL base CDN **cdnList** para fornecer a versão somente leitura atendida por um CDN. Somente leitura. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| cdnList | Coleção String | Uma lista de URLs base para todos os provedores CDN disponíveis que estão servindo os ativos do recurso atual. Vários CDN provedores são usados ao mesmo tempo para alta disponibilidade de solicitações de leitura. Somente leitura. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customAccountResetCredentialsUrl | Cadeia de caracteres | Uma URL personalizada para redefinir credenciais de conta. Essa URL deve estar no formato ASCII ou caracteres não ASCII devem ser codificados em URL e não exceder 128 caracteres. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customCannotAccessYourAccountText | Cadeia de caracteres | Uma cadeia de caracteres para substituir o padrão "Não é possível acessar sua conta?" texto de hiperlink de redefinição de senha de autoatendados (SSPR) na página de login. Este texto deve estar no formato Unicode e não exceder 256 caracteres. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customCannotAccessYourAccountUrl | Cadeia de caracteres | Uma URL personalizada para substituir a URL padrão da redefinição de senha de autoatendência (SSPR) "Não é possível acessar sua conta?" hiperlink na página de login. Essa URL deve estar no formato ASCII ou caracteres não ASCII devem ser codificados em URL e não exceder 128 caracteres. <br/><br/>**NÃO USE.** Use **customAccountResetCredentialsUrl** . Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customForgotMyPasswordText | Cadeia de caracteres | Uma cadeia de caracteres para substituir o texto padrão do hiperlink "Esqueci minha senha" no formulário de login. Este texto deve estar no formato Unicode e não exceder 256 caracteres. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customPrivacyAndCookiesText | Cadeia de caracteres | Uma cadeia de caracteres para substituir o texto padrão de hiperlink "Privacidade e Cookies" no rodapé. Este texto deve estar no formato Unicode e não exceder 256 caracteres. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customPrivacyAndCookiesUrl | Cadeia de caracteres | Uma URL personalizada para substituir a URL padrão do hiperlink "Privacidade e Cookies" no rodapé. Essa URL deve estar no formato ASCII ou caracteres não ASCII devem ser codificados em URL e não exceder 128 caracteres. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customResetItNowText | Cadeia de caracteres | Uma cadeia de caracteres para substituir o texto padrão do hiperlink "redefini-lo agora" no formulário de login. Este texto deve estar no formato Unicode e não exceder 256 caracteres. <br/><br/>**NÃO USE:** No momento, não há suporte para personalização do texto do hiperlink "redefini-lo agora". Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customTermsOfUseText | Cadeia de caracteres | Uma cadeia de caracteres para substituir o texto padrão de hiperlink "Termos de Uso" no rodapé. Este texto deve estar no formato Unicode e não exceder 256 caracteres. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| customTermsOfUseUrl | Cadeia de caracteres | Uma URL personalizada para substituir a URL padrão do hiperlink "Termos de Uso" no rodapé. Essa URL deve estar no formato ASCII ou caracteres não ASCII devem ser codificados por URL e não exceder 128characters. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| favicon | Stream | Um ícone personalizado (favicon) para substituir um favicon de produto padrão da Microsoft em um locatário do Azure AD. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| faviconRelativeUrl | Cadeia de caracteres | Uma URL relativa para o favicon acima que é combinada com uma URL CDN base da **cdnList** para fornecer a versão atendida por um CDN. Somente leitura. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| headerBackgroundColor | Cadeia de caracteres | A cor RGB a ser aplicada para personalizar a cor do header. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| id | Cadeia de caracteres | Um identificador que representa a localidade especificada usando nomes de cultura. Os nomes de cultura seguem o padrão RFC 1766 no formato "languagecode2-country/regioncode2", onde "languagecode2" é um código de duas letras minúsculo derivado da ISO 639-1 e "country/regioncode2" é um código de duas letras maiúscula derivado da ISO 3166. Por exemplo, inglês dos EUA é `en-US`. A **id para** o padrão /branding é sempre os tipos de cadeia de caracteres `0` ou `default`. Somente leitura. <br/><br/>**OBSERVAÇÃO:** No momento, não há suporte para várias marcas para uma única localidade. |
| loginPageTextVisibilitySettings | [loginPageTextVisibilitySettings](loginPageTextVisibilitySettings.md) | Representa os vários textos que podem ser ocultos na página de logon de um locatário. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| signInPageText | Cadeia de caracteres | Texto que aparece na parte inferior da caixa de login. Use isso para comunicar informações adicionais, como o número de telefone para sua assistência médica ou uma declaração legal. Este texto deve estar no formato Unicode e não exceder 1024 caracteres. |
| squareLogo | Stream | Uma versão quadrada do logotipo da sua empresa que aparece Windows 10 experiências in-loco (OOBE) e quando o Windows Autopilot está habilitado para implantação. Os tipos permitidos são PNG ou JPEG não maiores que 240 x 240 pixels e não mais de 10 KB de tamanho. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md).|
| squareLogoRelativeUrl | Cadeia de caracteres | Uma URL relativa para a **propriedade squareLogo** combinada com uma URL base CDN **cdnList** para fornecer a versão atendida por um CDN. Somente leitura. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |
| usernameHintText | Cadeia de caracteres | Uma cadeia de caracteres que mostra como a dica na caixa de texto do nome de usuário na tela de entrada. Este texto deve ser um Unicode, sem links ou código, e não pode exceder 64 caracteres. Herdado [de organizationalBrandingProperties](organizationalbrandingproperties.md). |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organizationalBrandingLocalization",
  "baseType": "microsoft.graph.organizationalBrandingProperties",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organizationalBrandingLocalization",
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
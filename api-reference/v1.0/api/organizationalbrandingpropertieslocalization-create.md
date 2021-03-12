---
title: Criar organizationalBrandingProperties localizados
description: Crie a identidade visual da organização para uma localidade específica.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8a52e0861f27fc1a21a87d23704d5163456a53ea
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722505"
---
# <a name="create-localized-organizationalbrandingproperties"></a>Criar organizationalBrandingProperties localizados

Crie um [objeto organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) para uma localidade específica.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Organization.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

POST para identidade visual/localizações para criar uma nova localização. A id especificada no corpo é a localidade da localização. Se nenhuma id for especificada, o valor do header Content-Language, se especificado, será usado como id. Se nenhuma id e nenhum header content-Language for especificado, um erro será retornado.
<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/branding/localizations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json. Obrigatório.  |
| Content-Language  | Localidade. Opcional.  |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|backgroundColor|Cadeia de caracteres|Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda. A cor primária do logotipo da faixa ou da cor da sua organização é recomendada para ser usada aqui. Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).|
|backgroundImage|Fluxo|Imagem que aparece como o plano de fundo da página de logom. .png ou .jpg não maior que 1920x1080 e menor que 300kb. Uma imagem menor reduzirá os requisitos de largura de banda e tornará as cargas de página mais performant.|
|bannerLogo|Fluxo|Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada. .png ou .jpg não maior que 36x245px. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.|
|signInPageText|Cadeia de caracteres|Texto que aparece na parte inferior da caixa de login. Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal. Este texto deve ser Unicode e não exceder 1024 caracteres.|
|squareLogo|Fluxo|Versão quadrada do logotipo da sua empresa. Isso aparece nas experiências OOBE (windows 10 out-of-box) e quando o Windows Autopilot está habilitado para implantação. .png ou .jpg não maior do que 240x240px e no máximo 10kb de tamanho. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.|
|usernameHintText|Cadeia de caracteres|Cadeia de caracteres que mostra como a dica na caixa de texto do nome de usuário na tela de entrada. Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.|
|id|Cadeia de caracteres|Localidade para criar identidade visual para|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) criado no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir cria uma localização de identidade visual para francês (fr).

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
POST https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr"
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": null,
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo"
}
```
O **mediaEditLink** especifica onde a mídia localizada é escrita. O mediaReadLink é nulo porque nenhuma mídia foi definida para a localização.

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

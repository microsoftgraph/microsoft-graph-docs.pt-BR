---
title: Criar organizationalBrandingProperties
description: Criar identidade visual da organização.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6f5e16a87f78be5e0664af624d058fff64f70bba
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722514"
---
# <a name="create-organizationalbrandingproperties"></a>Criar organizationalBrandingProperties

Crie um [objeto organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md) Isso cria a identidade visual padrão e, opcionalmente, uma identidade visual localizada. A identidade visual padrão é carregada quando um conjunto de identidade visual localizado não é configurado para o idioma do navegador do usuário.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Organization.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

Uma identidade visual é criada para uma organização, se ainda não existir, usando PUT ou PATCH.

Se a identidade visual já estiver configurada, PUT substituirá todos os valores existentes independentemente do que está no corpo da solicitação. PATCH apenas substitui os valores incluídos no corpo da solicitação, deixando os valores não incluídos inalterados.

A `id` propriedade é ignorada em PUT/PATCH no singleton /branding. Se **Content-Language** não for especificado, a identidade visual padrão será criada, o que corresponde a `id` um de `und` . Se **Content-Language** for especificado, a identidade visual será criada para essa localidade.
<!-- { "blockType": "ignored" } -->

```http
PUT /organization/{id}/branding
PATCH /organization/{id}/branding
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json. Obrigatório.  |
| Content-Language  | Localidade. Opcional.  |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, inclua uma representação JSON de um [objeto organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md) A tabela a seguir lista as propriedades necessárias.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|backgroundColor|Cadeia de caracteres|Cor que aparece no lugar da imagem de plano de fundo em conexões de baixa largura de banda. A cor primária do logotipo da faixa ou da cor da sua organização é recomendada para ser usada aqui. Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).|
|backgroundImage|Fluxo|Imagem que aparece como o plano de fundo da página de login. A imagem é um .png ou .jpg que não é maior que 1920x1080 e menor que 300kb. Uma imagem menor reduzirá os requisitos de largura de banda e tornará as cargas de página mais performant.|
|bannerLogo|Fluxo|Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada. O banner é um .png ou .jpg não maior que 36x245px. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.|
|signInPageText|Cadeia de caracteres|Texto que aparece na parte inferior da caixa de login. Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal. Este texto deve ser Unicode e não exceder 1024 caracteres.|
|squareLogo|Fluxo|Versão quadrada do logotipo da sua empresa. Isso aparece nas experiências OOBE (windows 10 out-of-box) e quando o Windows Autopilot está habilitado para implantação. O logotipo é um .png ou .jpg não maior que 240x240px e não mais de 10kb de tamanho. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.|
|usernameHintText|Cadeia de caracteres|A dica na caixa de texto nome de usuário na tela de entrada. Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) criado no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir cria a identidade visual padrão e a localização onde **Content-Language** é `en-US` .

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
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
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id": "und",
    "signInPageText":"Welcome",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "usernameHintText":"hint"
}
```

Nesse caso, o objeto de identidade visual padrão é definido. A identidade visual localizada para também é definida devido ao `en-US` header **Content-Language,** mesmo que o conjunto de identidade visual não seja `en-US` retornado na resposta. O **header Content-Language** na solicitação é opcional e, se não estiver presente, define apenas a identidade visual padrão.

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

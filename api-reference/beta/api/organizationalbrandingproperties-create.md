---
title: Criar organizationalBrandingProperties
description: Criar identidade visual da organização.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: efb10cd5669022dda2afd385ea013ae110a97ea0
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031912"
---
# <a name="create-organizationalbrandingproperties"></a>Criar organizationalBrandingProperties

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar um objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) . Isso cria a identidade visual padrão e, opcionalmente, uma identidade visual localizada ao mesmo tempo. A identidade visual padrão é carregada quando um conjunto de identidade visual localizado não é configurado para o idioma do navegador do usuário.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Organization.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

Uma identidade visual é criada para uma organização, se ainda não existir uma, usando PUT ou PATCH.

Se a identidade visual já estiver configurada, PUT substituirá todos os valores existentes, independentemente do que está no corpo da solicitação. O PATCH só overite os valores que estão incluídos no corpo da solicitação, deixando os valores não incluídos inalterados.

A propriedade **ID** é ignorada em Put/patch para o singleton/branding. Se Content-Language não for especificado, a identidade visual padrão será criada, o que corresponde a uma **ID** de `und` . Se o idioma de conteúdo for especificado, a identidade visual será criada para essa localidade.
<!-- { "blockType": "ignored" } -->

```http
PUT /organization/{id}/branding
PATCH /organization/{id}/branding
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json. Obrigatório.  |
| Conteúdo-idioma  | LCID. Opcional.  |

## <a name="request-body"></a>Corpo da solicitação

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|CorDoFundo|String|Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda. É recomendável usar a cor principal do logotipo de faixa ou a cor da sua organização aqui. Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).|
|backgroundImage|Fluxo|Imagem que aparece como plano de fundo da página de entrada. . png ou. jpg não é maior do que 1920 x 1080 e menor do que 300kb. Uma imagem menor reduzirá os requisitos de largura de banda e fará com que as cargas de página mais tenham mais desempenho.|
|bannerLogo|Fluxo|Uma versão de banner do logotipo da empresa que aparece aparece na página de entrada. . png ou. jpg não maior do que 36x245px. Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo.|
|signInPageText|String|Texto que aparece na parte inferior da caixa de entrada. Você pode usá-lo para comunicar informações adicionais, como o número de telefone para o suporte técnico ou uma instrução legal. Este texto deve ser Unicode e não exceder 1024 caracteres.|
|squareLogo|Fluxo|Versão quadrada do logotipo da sua empresa. Isso aparece nas experiências de uso (OOBE) do Windows 10 e quando o Windows AutoPilot está habilitado para implantação. . png ou. jpg não maior do que 240x240px e não mais do que 10 KB em tamanho. Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo.|
|usernameHintText|String|Cadeia de caracteres que mostra como a dica na caixa de texto username na tela de entrada. Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) criado no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir cria a identidade visual e a localização padrão para en-US.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
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
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id": "und",
    "signInPageText":"Welcome",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "usernameHintText":"hint"
}
```

Nesse caso, o objeto de identidade visual padrão é definido. A identidade visual localizada para en-US também é definida devido ao idioma do conteúdo no cabeçalho, mesmo que o conjunto de marcas en-US não seja retornado na resposta. Observe que o idioma de conteúdo na solicitação é opcional e, se não estiver presente, só definirá a identidade visual padrão.

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

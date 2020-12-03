---
title: Criar organizationalBrandingProperties localizado
description: Crie uma identidade visual da organização para uma localidade específica.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4c293085887eb0e8c2d49c4e01c567dbeea32699
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49524418"
---
# <a name="create-localized-organizationalbrandingproperties"></a>Criar organizationalBrandingProperties localizado

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) para uma localidade específica.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | Organization.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

POSTAR na identidade visual/localizações para criar uma nova localização. A ID especificada no corpo é a localidade para a localização. Se nenhuma ID for especificada, o valor do cabeçalho de idioma de conteúdo, se especificado, será usado como a ID. Se não houver nenhuma ID e cabeçalho de idioma de conteúdo especificado, um erro será retornado.
<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/branding/localizations
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

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|CorDoFundo|String|Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda. É recomendável usar a cor principal do logotipo de faixa ou a cor da sua organização aqui. Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).|
|backgroundImage|Stream|Imagem que aparece como plano de fundo da página de entrada. . png ou. jpg não é maior do que 1920 x 1080 e menor do que 300kb. Uma imagem menor reduzirá os requisitos de largura de banda e fará com que as cargas de página mais tenham mais desempenho.|
|bannerLogo|Stream|Uma versão de banner do logotipo da empresa que aparece aparece na página de entrada. . png ou. jpg não maior do que 36x245px. Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo.|
|signInPageText|String|Texto que aparece na parte inferior da caixa de entrada. Você pode usá-lo para comunicar informações adicionais, como o número de telefone para o suporte técnico ou uma instrução legal. Este texto deve ser Unicode e não exceder 1024 caracteres.|
|squareLogo|Stream|Versão quadrada do logotipo da sua empresa. Isso aparece nas experiências de uso (OOBE) do Windows 10 e quando o Windows AutoPilot está habilitado para implantação. . png ou. jpg não maior do que 240x240px e não mais do que 10 KB em tamanho. Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo.|
|usernameHintText|String|Cadeia de caracteres que mostra como a dica na caixa de texto username na tela de entrada. Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.|
|id|String|Local para criar identidade visual para|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 CREATED` código de resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) criado no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir cria uma localização de identidade visual para francês (FR).

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
POST https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo"
}
```
O **mediaEditLink** especifica onde a mídia localizada foi gravada. O mediaReadLink é NULL porque nenhuma mídia foi definida para a localização.

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

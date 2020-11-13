---
title: Atualizar organizationalbrandingproperties localizado
description: Atualize as propriedades do objeto organizationalbrandingproperties para uma localização específica.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0b835316d611d3735a0a981fc77f58622ab89c9b
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031891"
---
# <a name="update-localized-organizationalbrandingproperties"></a>Atualizar organizationalbrandingproperties localizado

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades do objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) para uma localização específica.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Organization.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/localizations/{locale}/{property name}
PUT /organization/{id}/branding/localizations/{locale}/{property name}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json. Obrigatório.  |
| Conteúdo-idioma  | LCID. Opcional.  |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|CorDoFundo|String|Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda. É recomendável usar a cor principal do logotipo de faixa ou a cor da sua organização aqui. Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).|
|backgroundImage|Fluxo|Imagem que aparece como plano de fundo da página de entrada. . png ou. jpg não é maior do que 1920 x 1080 e menor do que 300kb. Uma imagem menor reduzirá os requisitos de largura de banda e fará com que as cargas de página mais tenham mais desempenho.|
|bannerLogo|Fluxo|Uma versão de banner do logotipo da empresa que aparece aparece na página de entrada. . png ou. jpg não maior do que 36x245px. Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo.|
|signInPageText|String|Texto que aparece na parte inferior da caixa de entrada. Você pode usá-lo para comunicar informações adicionais, como o número de telefone para o suporte técnico ou uma instrução legal. Este texto deve ser Unicode e não exceder 1024 caracteres.|
|squareLogo|Fluxo|Versão quadrada do logotipo da sua empresa. Isso aparece nas experiências de uso (OOBE) do Windows 10 e quando o Windows AutoPilot está habilitado para implantação. . png ou. jpg não maior do que 240x240px e não mais do que 10 KB em tamanho. Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo.|
|usernameHintText|String|Cadeia de caracteres que mostra como a dica na caixa de texto username na tela de entrada. Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.|
|id|String|Local para atualizar a identidade visual do|


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 OK`.

## <a name="examples"></a>Exemplos

### <a name="example-1-setting-bannerlogo-for-the-fr-localization-using-put"></a>Exemplo 1: Configurando **bannerLogo** para a localização fr usando put

A solicitação a seguir atualiza o logotipo do banner para a localização fr. Usando PUT, se a localização fr não existir, "404 não encontrado" será retornado. Se a carga contiver uma propriedade ID ou cabeçalho de linguagem de conteúdo e não corresponder à ID na URL, uma solicitação inválida será retornada.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

### <a name="example-2-update-bannerlogo-for-the-fr-localization-using-patch"></a>Exemplo 2: atualizar **bannerLogo** para a localização fr usando patch

A solicitação a seguir atualiza o logotipo do banner para a localização fr.  Usando PATCH, se a localização especificada ainda não existir, ela será criada e a propriedade será gravada nela.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```

#### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```



### <a name="example-3-override-default-branding-value-with-a-blank-string"></a>Exemplo 3: substituir o valor padrão de identidade visual por uma cadeia de caracteres em branco

Se o valor de uma propriedade em uma localização for nulo, o valor será herdado da identidade visual padrão. Para evitar que isso aconteça, defina uma cadeia de caracteres vazia ou uma cadeia de caracteres contendo apenas espaços em branco na identidade visual localizada.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "signInPageText": "French sign-in text.",
    "usernameHintText":" "
}
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

Após essa solicitação, usernameHintText para a localização fr estará vazia em vez de herdar o valor da identidade visual padrão.

### <a name="example-4-replace-french-localization-with-put"></a>Exemplo 4: substituir a localização em francês por PUT

Para fazer uma atualização na localização usando PUT, devemos adicionar todas as propriedades no corpo junto com a propriedade que precisa ser atualizada conforme PUT substitui o objeto existente pelo novo. As outras propriedades que não estão no corpo de carga de PUT serão definidas como NULL. Aqui, no exemplo abaixo, somente a propriedade backgroundColor é mantida e o signInPageText é atualizado enquanto outros são definidos como NULL.
Se a localização especificada ainda não existir, coloque na URL especificando que a localização a cria.
Se a carga contiver uma propriedade ID ou um cabeçalho de idioma de conteúdo e não corresponder à ID na URL, lançamos uma solicitação incorreta.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```

#### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
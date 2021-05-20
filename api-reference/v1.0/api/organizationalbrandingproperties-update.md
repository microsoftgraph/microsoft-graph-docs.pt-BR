---
title: Atualizar organizaçõesMarcas de marcaçãoProvas
description: Atualize as propriedades de um objeto organizacionalBrandingProperties.
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 95bf7425fff3ac48bd74920d7792e56d0d360f82
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547222"
---
# <a name="update-organizationalbrandingproperties"></a>Atualizar organizaçõesMarcas de marcaçãoProvas

Atualize as propriedades de um objeto [organizacionalBrandingProperties.](../resources/organizationalbrandingproperties.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | Organization.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{tenant id}/branding/{property name}
PUT /organization/{tenant id}/branding/{property name}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json. Obrigatório.  |
| Linguagem de conteúdo  | localidade. Opcional.  |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|backgroundColor|Cadeia de caracteres|Cor que aparecerá no lugar da imagem de fundo em conexões de baixa largura de banda. Recomenda-se que a cor principal do logotipo do seu banner ou da sua organização seja usada aqui. Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).|
|backgroundImage|Stream|Imagem que aparece como o fundo do sinal na página. .png ou .jpg não maior que 1920x1080 e menor que 300kb. Uma imagem menor reduzirá os requisitos de largura de banda e tornará as cargas de página mais executantes.|
|bannerLogo|Stream|Uma versão de banner do logotipo da sua empresa que aparece aparece na página de login. .png ou .jpg não maior que 36x245px. Recomendamos o uso de uma imagem transparente sem estofamento ao redor do logotipo.|
|signInPageText|Cadeia de caracteres|Texto que aparece na parte inferior da caixa de entrada. Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal. Este texto deve ser Unicode e não exceder 1024 caracteres.|
|squareLogo|Stream|Versão quadrada do logotipo da sua empresa. Isso aparece em Windows 10 experiências fora da caixa (OOBE) e quando Windows Piloto Automático está habilitado para implantação. .png ou .jpg não maior que 240x240px e não mais do que 10kb de tamanho. Recomendamos o uso de uma imagem transparente sem estofamento ao redor do logotipo.|
|nome de usuárioHintText|Cadeia de caracteres|String que mostra como a dica na caixa de texto do nome de usuário na tela do sinal. Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.|

A propriedade **de id** é ignorada quando passou dentro

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos
### <a name="example-1-update-default-branding"></a>Exemplo 1: Atualizar a marca padrão
Se a marca já existir, `PATCH` substituirá apenas as propriedades especificadas, deixando as propriedades não especificadas inalteradas. 
#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_1"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 OK
```

Neste caso, os valores da marca padrão são atualizados, mas nenhum valor é alterado em qualquer localização.

### <a name="example-2-update-bannerlogo-for-default-branding"></a>Exemplo 2: Atualizar bannerLogo para marca padrão
A solicitação a seguir atualiza o logotipo do banner para a marca padrão.
#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_2"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
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
HTTP/1.1 204 No Content
```

### <a name="example-3-update-localized-branding"></a>Exemplo 3: Atualizar marca localizada
Se o cabeçalho **de linguagem de conteúdo** for especificado, a localização associada ao **Conteúdo-Linguagem** será primeiramente criada se ela ainda não existir e, em seguida, atualizada usando os valores especificados. A marca padrão não é alterada.
#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_3"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
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

Após essa solicitação, a `fr` localização é atualizada com o novo valor de **backgroundColor,** mas nenhuma alteração é feita na marca padrão.

### <a name="example-4-replace-default-branding-and-all-localizations"></a>Exemplo 4: Substituir a marca padrão e todas as localizações
Se a marca já existir, `PUT` substituirá a marca padrão e quaisquer localizações.
#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_4"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

Após essa solicitação, a marca padrão tem apenas o **backgroundColor** especificado e tem exatamente uma localização com o **id** `fr` , também com o conjunto **backgroundColor.**
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

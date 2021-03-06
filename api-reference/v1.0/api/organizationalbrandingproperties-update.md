---
title: Atualizar organizationalBrandingProperties
description: Atualize as propriedades de um objeto organizationalBrandingProperties.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1fd15c3ae41af043cb7c5163d8b7ac8b06a36ae0
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722506"
---
# <a name="update-organizationalbrandingproperties"></a>Atualizar organizationalBrandingProperties

Atualize as propriedades de [um objeto organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Organization.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/{property name}
PUT /organization/{id}/branding/{property name}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
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

A `id` propriedade é ignorada quando passada.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos
### <a name="example-1-update-default-branding"></a>Exemplo 1: atualizar a identidade visual padrão
Se a identidade visual já existir, PATCH substituirá apenas as propriedades especificadas, deixando propriedades não especificadas inalteradas. 
#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
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
HTTP/1.1 204 OK
```

Nesse caso, os valores do padrão /branding são atualizados, mas nenhum valor é alterado em qualquer localização.

### <a name="example-2-update-bannerlogo-for-default-branding"></a>Exemplo 2: Atualizar bannerLogo para identidade visual padrão
A solicitação a seguir atualiza o logotipo da faixa para a identidade visual padrão.
#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
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

### <a name="example-3-update-localized-branding"></a>Exemplo 3: atualizar a identidade visual localizada
Se o header content-Language for especificado, a localização associada ao Content-Language será criada, se ainda não existir e, em seguida, atualizada usando os valores especificados. A identidade visual padrão não foi alterada.
#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
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

Após essa solicitação, a localização fr é atualizada com o novo valor de backgroundColor, mas nenhuma alteração é feita para o padrão /branding.

### <a name="example-4-replace-default-branding-and-all-localizations"></a>Exemplo 4: Substituir a identidade visual padrão e todas as localizações
Se a identidade visual já existir, PUT substituirá a identidade visual padrão e quaisquer localizações.
#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
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

Após essa solicitação, a identidade visual padrão tem apenas o backgroundColor especificado e tem exatamente uma localização com o id fr, também com o conjunto backgroundColor.
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

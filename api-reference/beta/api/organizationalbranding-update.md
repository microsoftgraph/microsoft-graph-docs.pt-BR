---
title: Atualizar organizationalBranding
description: Atualize as propriedades de um objeto organizationalBranding.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: db77089b1da77420111c9dda30264e4fab89296d
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777330"
---
# <a name="update-organizationalbranding"></a>Atualizar organizationalBranding
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades do objeto de identidade visual padrão especificado pelo [objeto organizationalBranding.](../resources/organizationalbranding.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Organization.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}/branding
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|
|Accept-Language|Uma localidade ISO 639-1 válida. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece *apenas* os valores das propriedades que devem ser atualizadas. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. 

A tabela a seguir especifica as propriedades que podem ser atualizadas. 

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| backgroundColor | String | Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda. Recomendamos que você use a cor primária do logotipo da faixa ou da cor da sua organização. Especifique isso no formato hexadecimal, por exemplo, branco é `#FFFFFF` . |
| backgroundImage | Stream | Imagem que aparece como o plano de fundo da página de login. Os tipos permitidos são PNG ou JPEG não menores que 300 KB e não maiores que 1920 × 1080 pixels. Uma imagem menor reduzirá os requisitos de largura de banda e tornará a carga da página mais rápida. |
| bannerLogo | Stream | Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada. Os tipos permitidos são PNG ou JPEG não maiores que 36 × 245 pixels. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo. |
| signInPageText | String | Texto que aparece na parte inferior da caixa de login. Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal. Este texto deve ser Unicode e não exceder 1024 caracteres. |
| squareLogo | Stream | Uma versão quadrada do logotipo da sua empresa que aparece Windows 10 experiências in-loco (OOBE) e quando o Windows Autopilot está habilitado para implantação. Os tipos permitidos são PNG ou JPEG não maiores que 240 x 240 pixels e no máximo 10 KB de tamanho. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo. |
| usernameHintText | Cadeia de caracteres | Cadeia de caracteres que mostra como a dica na caixa de texto do nome de usuário na tela de entrada. Este texto deve ser um Unicode, sem links ou código, e não pode exceder 64 caracteres. |


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="example-1-update-the-default-branding"></a>Exemplo 1: atualizar a identidade visual padrão

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocaliation_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```


#### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-bannerlogo-for-default-branding"></a>Exemplo 2: Atualizar bannerLogo para identidade visual padrão

A solicitação a seguir atualiza o logotipo da faixa para a identidade visual padrão.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocaliation_2"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

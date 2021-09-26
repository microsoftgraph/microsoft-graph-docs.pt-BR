---
title: Obter organizationalBranding
description: Leia as propriedades e as relações de um objeto organizationalBranding.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9f23d7f22e11a5c2e80189d843071c30ddd6d568
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777327"
---
# <a name="get-organizationalbranding"></a>Obter organizationalBranding
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere o objeto de identidade visual organizacional padrão, se o header **Accept-Language** não for especificado. Se nenhum objeto de identidade visual organizacional tiver sido criado, este método retornará um `404 Not Found` erro.

Se o header **Accept-Language** for especificado, esse método recuperará a identidade visual da localidade especificada.

Este método recupera apenas propriedades que não são stream, por exemplo, **usernameHintText** e **signInPageText**. Para recuperar tipos stream da identidade visual padrão, por exemplo, **bannerLogo** e **backgroundImage**, use o [método GET organizationalBrandingLocalization.](organizationalbrandinglocalization-get.md) A **id** da localização padrão pode ser `0` ou `default` .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | User.Read, Organization.Read.All, User.ReadBasic.All, User.Read.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}/branding
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte apenas ao `$select` parâmetro de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Accept-Language|Uma localidade ISO 639-1 válida. Opcional.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [organizationalBranding](../resources/organizationalbranding.md) no corpo da resposta. Se nenhum objeto de identidade visual padrão existir, este método retornará um `404 Not Found` código de resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-the-default-branding"></a>Exemplo 1: Obter a identidade visual padrão

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/84841066-274d-4ec0-a5c1-276be684bdd3/branding
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBranding"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#branding",
    "@odata.id": "https://graph.microsoft.com/v2/99b24e1b-abec-4598-9d63-a2baf0a3cea1/directoryObjects/$/Microsoft.DirectoryServices.Organization('99b24e1b-abec-4598-9d63-a2baf0a3cea1')/branding/0",
    "id": "0",
    "backgroundColor": "",
    "backgroundImageRelativeUrl": "c1c6b6c8-urr-dzbkz44n5kuo9kzl1kziuujjcdqonoe2owyacso/logintenantbranding/0/illustration?ts=637535563816027796",
    "bannerLogoRelativeUrl": "c1c6b6c8-urr-dzbkz44n5kuo9kzl1kziuujjcdqonoe2owyacso/logintenantbranding/0/bannerlogo?ts=637535563824629275",
    "cdnList": [
        "secure.aadcdn.microsoftonline-p.com",
        "aadcdn.msftauthimages.net",
        "aadcdn.msauthimages.net"
    ],
    "signInPageText": "Contoso",
    "squareLogoRelativeUrl": "c1c6b6c8-urr-dzbkz44n5kuo9kzl1kziuujjcdqonoe2owyacso/logintenantbranding/0/tilelogo?ts=637535563832888580",
    "usernameHintText": ""
}
```


### <a name="example-2-get-organizational-branding-when-no-branding-is-configured"></a>Exemplo 2: Obter identidade visual organizacional quando nenhuma identidade visual estiver configurada

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding_Error"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 404 Not Found
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a>Exemplo 3: Obter identidade visual organizacional para a localidade francesa

No exemplo a seguir, o header **Accept-Language** é usado para especificar a identidade visual de localização a ser recuperada.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding_locale"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr-FR
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBranding"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#branding",
    "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/$/Microsoft.DirectoryServices.Organization('84841066-274d-4ec0-a5c1-276be684bdd3')/branding/fr",
    "id": "fr",
    "backgroundColor": "#FFFF33",
    "backgroundImageRelativeUrl": null,
    "bannerLogoRelativeUrl": null,
    "cdnList": [],
    "signInPageText": " ",
    "squareLogoRelativeUrl": null,
    "usernameHintText": " "
}
```

### <a name="example-4-get-the-bannerlogo-for-the-default-locale"></a>Exemplo 4: Obter o bannerLogo para a localidade padrão

O exemplo a seguir retorna o **objeto bannerLogo** para a localidade padrão. Você pode especificar **a id** como `default` ou na URL da `0` solicitação. Se o objeto não estiver definido, a solicitação retornará uma resposta vazia.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "ignored",
  "name": "get_organizationalbranding_defaultlocale_bannerLogo"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/default/bannerLogo
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBranding"
} -->

```http
HTTP/1.1 200 OK
Content-Type: image/*

<Image>
```

### <a name="example-5-get-the-bannerlogo-for-the-fr-fr-locale"></a>Exemplo 5: Obter o bannerLogo para a localidade fr-FR

O exemplo a seguir retorna o **objeto bannerLogo** para `fr-FR` a localidade cujo bannerLogo não está definido.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding_frlocale_bannerLogo"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/default/bannerLogo
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBranding"
} -->

```http
HTTP/1.1 200 OK

{}
```

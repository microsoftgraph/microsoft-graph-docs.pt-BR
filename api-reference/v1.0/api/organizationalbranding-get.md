---
title: Obter organizationalBranding
description: Leia as propriedades e as relações de um objeto organizationalBranding.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 560e9fecde0770bbc53c888b994653a7ebfe6755
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027351"
---
# <a name="get-organizationalbranding"></a>Obter organizationalBranding
Namespace: microsoft.graph

Recupere o objeto de identidade visual organizacional padrão, se o header **Accept-Language** estiver definido como `0` ou `default` . Se nenhum objeto de identidade visual organizacional padrão existir, este método retornará um `404 Not Found` erro.

Se o header **Accept-Language** for definido como uma localidade existente identificada pelo valor de sua **id,** este método recuperará a identidade visual da localidade especificada.

Este método recupera apenas propriedades que não são stream, por exemplo, **usernameHintText** e **signInPageText**. Para recuperar tipos stream da identidade visual padrão, por exemplo, **bannerLogo** e **backgroundImage**, use o [método GET organizationalBrandingLocalization.](organizationalbrandinglocalization-get.md)

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
|Accept-Language|Uma localidade ISO 639-1 válida. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [organizationalBranding](../resources/organizationalbranding.md) no corpo da resposta. Se nenhum objeto de identidade visual padrão existir, este método retornará um `404 Not Found` código de resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-the-default-branding"></a>Exemplo 1: Obter a identidade visual padrão

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/84841066-274d-4ec0-a5c1-276be684bdd3/branding
Accept-Language: 0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbranding-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbranding-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbranding-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbranding-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-organizationalbranding-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#branding",
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

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding_Error"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: 0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbranding-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbranding-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbranding-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbranding-error-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-organizationalbranding-error-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 404 Not Found
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a>Exemplo 3: Obter identidade visual organizacional para a localidade francesa

No exemplo a seguir, o header **Accept-Language** é usado para especificar para recuperar a `fr-FR` identidade visual de localização.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding_locale"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr-FR
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbranding-locale-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbranding-locale-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbranding-locale-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbranding-locale-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-organizationalbranding-locale-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#branding",
    "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/$/Microsoft.DirectoryServices.Organization('84841066-274d-4ec0-a5c1-276be684bdd3')/branding/fr-FR",
    "id": "fr-FR",
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

O exemplo a seguir retorna o **objeto bannerLogo** para a localidade padrão. Para recuperar tipos de objeto Stream, por exemplo, **bannerLogo**, use [o get organizationalBrandingLocalizationmethod](organizationalbrandinglocalization-get.md). Você pode especificar o valor da **id** como `default` ou na URL da `0` solicitação. Se a propriedade não estiver definida, a solicitação retornará uma resposta vazia.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "ignored",
  "name": "get_organizationalbranding_defaultlocale_bannerLogo"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/default/bannerLogo
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

### <a name="example-5-get-the-bannerlogo-for-the-default-locale-when-it-is-not-set"></a>Exemplo 5: Obter o bannerLogo para a localidade padrão quando ele não estiver definido

O exemplo a seguir retorna o **objeto bannerLogo** que não foi definido para a localidade padrão.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding_frlocale_bannerLogo"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/default/bannerLogo
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbranding-frlocale-bannerlogo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbranding-frlocale-bannerlogo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbranding-frlocale-bannerlogo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbranding-frlocale-bannerlogo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

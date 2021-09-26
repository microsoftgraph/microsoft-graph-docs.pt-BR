---
title: Obter organizationalBrandingLocalization
description: Leia as propriedades e as relações de um objeto organizationalBrandingLocalization.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 767b6a73c26a12e3451671b445baab17b0b3bbdf
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777348"
---
# <a name="get-organizationalbrandinglocalization"></a>Obter organizationalBrandingLocalization
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto organizationalBrandingLocalization.](../resources/organizationalbrandinglocalization.md) Para recuperar um objeto de identidade visual de localização, especifique o valor da **id** na URL.

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
GET /organization/{organizationId}/branding/localizations/{organizationalBrandingLocalizationId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-the-localized-branding-for-a-specific-locale-fr-fr"></a>Exemplo 1: Obter a identidade visual localizada para uma localidade específica (fr-FR)

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandinglocalization"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR
```


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingLocalization"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization('99b24e1b-abec-4598-9d63-a2baf0a3cea1')/branding/localizations/$entity",
    "@odata.type": "#microsoft.graph.organizationalBrandingProperties",
    "@odata.id": "https://graph.microsoft.com/v2/99b24e1b-abec-4598-9d63-a2baf0a3cea1/directoryObjects/$/Microsoft.DirectoryServices.Organization('99b24e1b-abec-4598-9d63-a2baf0a3cea1')//localizations('fr-FR')/fr-FR",
    "id": "fr-FR",
    "backgroundColor": "",
    "backgroundImageRelativeUrl": null,
    "bannerLogoRelativeUrl": "c1c6b6c8-urr-dzbkz44n5kuo9kzl1kziuujjcdqonoe2owyacso/logintenantbranding/1036/bannerlogo?ts=637673868626068858",
    "cdnList": [
        "secure.aadcdn.microsoftonline-p.com",
        "aadcdn.msftauthimages.net",
        "aadcdn.msauthimages.net"
    ],
    "signInPageText": "Welcome to Contoso France",
    "usernameHintText": "Welcome to Contoso France"
}
```

### <a name="example-2-get-the-value-of-signinpagetext-for-a-specific-locale"></a>Exemplo 2: Obter o valor de signInPageText para uma localidade específica

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandinglocalization_locale_signInPageText"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/99b24e1b-abec-4598-9d63-a2baf0a3cea1/branding/localizations/fr-FR/signInPageText
```


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingLocalization"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization('99b24e1b-abec-4598-9d63-a2baf0a3cea1')/branding/localizations('fr-FR')/usernameHintText",
    "value": "Welcome to Contoso France"
}
```

### <a name="example-3-get-the-bannerlogo-for-the-default-locale"></a>Exemplo 3: Obter o bannerLogo para a localidade padrão

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

### <a name="example-4-get-the-bannerlogo-for-the-fr-fr-locale"></a>Exemplo 4: Obter o bannerLogo para a localidade fr-FR

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

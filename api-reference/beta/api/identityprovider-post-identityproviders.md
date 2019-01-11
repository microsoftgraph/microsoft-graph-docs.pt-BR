---
title: Criar identityProvider
description: Crie um novo identityProvider especificando o nome para exibição, tipo de identityProvider, ID de cliente e segredo do cliente.
localization_priority: Normal
ms.openlocfilehash: 50ead5acbbda7725e44de55865d6fe2184c89647
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866231"
---
# <a name="create-identityprovider"></a>Criar identityProvider

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Crie um novo [identityProvider](../resources/identityprovider.md) especificando o nome para exibição, tipo de identityProvider, ID de cliente e segredo do cliente.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)|IdentityProvider.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|Sem suporte.|

A conta do trabalho ou da escola deve ser um administrador global do inquilino.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---------------|:----------|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornecem uma representação de JSON do objeto [identityProvider](../resources/identityprovider.md) . Todas as propriedades listadas na tabela a seguir são necessárias.

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|A identificação do cliente para o aplicativo. Esta é a ID de cliente obtida ao registrar o aplicativo com o provedor de identidade.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo. Esse é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.|
|name|Cadeia de caracteres|O nome de exibição do provedor de identidade.|
|type|Cadeia de caracteres|O tipo de provedor de identidade. Ele deve ser um dos seguintes valores: <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook</ul>|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` objeto response de código e [identityProvider](../resources/identityprovider.md) no corpo da resposta. Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.

## <a name="example"></a>Exemplo

O exemplo a seguir cria um **identityProvider**.

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}-->
```http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

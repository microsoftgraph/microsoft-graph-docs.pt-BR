---
title: Criar certificateBasedAuthConfiguration
description: Use essa API para criar um novo certificateBasedAuthConfiguration.
ms.localizationpriority: medium
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 98bf11a685980a4976999369b18767c05c54d243
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59131025"
---
# <a name="create-certificatebasedauthconfiguration"></a>Criar certificateBasedAuthConfiguration

Namespace: microsoft.graph

Crie um novo [objeto certificateBasedAuthConfiguration.](../resources/certificateBasedAuthConfiguration.md)

> [!NOTE]
> Somente uma única instância de **um certificateBasedAuthConfiguration** pode ser criada (a coleção só pode ter um membro). Ele sempre tem uma ID fixa com um valor '29728ade-6ae4-4ee9-9103-412912537da5'.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | Organization.ReadWrite.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo    | Organization.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |
| Content-Type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

As propriedades a seguir são necessárias para criar o [objeto certificateBasedAuthConfiguration.](../resources/certificatebasedauthconfiguration.md)

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|certificateAuthorities| [Coleção certificateAuthority](../resources/certificateauthority.md) |Coleção de autoridades de certificados que cria uma cadeia de certificados confiável.  Cada membro da coleção deve conter **propriedades certificate** e **isRootAuthority.** |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará o código de resposta e `201 Created` um novo [objeto certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_certificatebasedauthconfiguration_from_certificatebasedauthconfiguration"
}-->

```http
POST https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration
Content-type: application/json

{
  "certificateAuthorities": [
    {
      "isRootAuthority": true,
      "certificate": "Binary"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "certificateAuthorities": [
    {
      "isRootAuthority": true,
      "certificate": "Binary",
      "issuer": "issuer-value",
      "issuerSki": "issuerSki-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


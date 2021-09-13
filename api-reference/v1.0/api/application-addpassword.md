---
title: 'application: addPassword'
description: Adicionar uma senha forte a um aplicativo.
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 6a90967358ff4acccdc33274fc689fd1998f24d6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59100502"
---
# <a name="application-addpassword"></a>application: addPassword

Namespace: microsoft.graph

Adiciona uma senha forte a um [aplicativo](../resources/application.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | Application.ReadWrite.All, Directory.AccessAsUser.All |
| Delegada (conta pessoal da Microsoft) | Application.ReadWrite.All |
| Aplicativo                            | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           | Descrição                |
|:---------------|:---------------------------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type   | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça um `passwordCredential` objeto opcional com as seguintes propriedades.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| displayName | Cadeia de caracteres | Nome amigável para a senha. Opcional. |
| endDateTime | DateTimeOffset | A data e a hora em que a senha expira representada usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Opcional. O valor padrão é "startDateTime + 2 anos". |
| startDateTime | DateTimeOffset | A data e a hora em que a senha se torna válida. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Opcional.  O valor padrão é "now". |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um novo objeto [passwordCredential](../resources/passwordcredential.md) no corpo da resposta. A **propriedade secretText** no objeto de resposta contém as senhas fortes geradas por Azure Active Directory que têm 16 a 64 caracteres de comprimento. Não há como recuperar essa senha no futuro.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. A **id** especificada na solicitação é o valor da propriedade **id** do aplicativo, não o valor da **propriedade appId.** 

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addpassword"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/addPassword
Content-type: application/json

{
  "passwordCredential": {
    "displayName": "Password friendly name"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addpassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addpassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-addpassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordCredential"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "customKeyIdentifier": null,
    "endDateTime": "2021-09-09T19:50:29.3086381Z",
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "startDateTime": "2019-09-09T19:50:29.3086381Z",
    "secretText": "[6gyXA5S20@MN+WRXAJ]I-TO7g1:h2P8",
    "hint": "[6g",
    "displayName": "Password friendly name"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: addPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


---
title: Criar extensionProperty
description: Crie uma nova extensionProperty.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 7105cce50e231280d88f1cf96289fa7cbc0fca94
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135839"
---
# <a name="create-extensionproperty"></a>Criar extensionProperty

Namespace: microsoft.graph

Crie uma nova [definição extensionProperty.](../resources/extensionproperty.md) Você pode usar essa operação para adicionar um valor de propriedade personalizado ao tipo de objeto de destino definido na **extensionProperty**, usando solicitações padrão de criação e atualização para o objeto de destino.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Application.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegada (conta pessoal da Microsoft) | Application.ReadWrite.All |
|Aplicativo | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/extensionProperties
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:-----------|:----------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça [um objeto extensionProperty](../resources/extensionproperty.md) com as propriedades a seguir.


| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|dataType|Cadeia de caracteres| Especifica o tipo de dados do valor que a propriedade de extensão pode conter. Os valores a seguir são suportados. Não anulável. <ul><li>`Binary` - Máximo de 256 bytes</li><li>`Boolean`</li><li>`DateTime` - Deve ser especificado no formato ISO 8601. Serão armazenados no UTC.</li><li>`Integer` - Valor de 32 bits.</li><li>`LargeInteger` - Valor de 64 bits.</li><li>`String` - Máximo de 256 caracteres</li></ul>|
|nome|String| Nome da propriedade de extensão. Não anulável. |
|targetObjects|String collection| Os valores a seguir são suportados. Não anulável. <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|


## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta e um novo objeto `201 Created` [extensionProperty](../resources/extensionproperty.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_extensionproperty_from_application"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties
Content-type: application/json

{
    "name": "extensionName",
    "dataType": "string",
    "targetObjects": [
        "Application"
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-extensionproperty-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-extensionproperty-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-extensionproperty-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-extensionproperty-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta e o `201 Created` [objeto extensionProperty](../resources/extensionProperty.md) no corpo da resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extensionProperty"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "a2c459db-f5dc-4328-ae9b-118e88d04d19",
    "deletedDateTime": null,
    "appDisplayName": "Display name",
    "name": "extension_b3efaf8f68a44275abcff28ef86b2ee3_extensionName",
    "dataType": "String",
    "isSyncedFromOnPremises": false,
    "targetObjects": [
        "Application"
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create extensionProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


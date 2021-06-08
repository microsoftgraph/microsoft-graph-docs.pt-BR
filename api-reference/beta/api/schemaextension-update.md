---
title: Update schemaExtension
description: Atualizar propriedades na definição do esquemaExtension especificado.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 6e5bef7a1ac978ccde1c84a9ee074d7fc6d91c28
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787371"
---
# <a name="update-schemaextension"></a>Update schemaExtension

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualizar propriedades na definição do [esquemaExtension especificado.](../resources/schemaextension.md) Atualizações aditivas para a extensão só podem ser feitas quando a extensão estiver no status **InDevelopment** ou **Disponível.** Isso significa que propriedades personalizadas ou tipos de recurso de destino não podem ser removidos da definição, mas novas propriedades personalizadas podem ser adicionadas e a descrição da extensão alterada.

A atualização se aplica a todos os recursos incluídos na **propriedade targetTypes** da extensão. Esses recursos estão entre os [tipos de recursos de suporte.](/graph/extensibility-overview#supported-resources)

Para fluxos delegados, o usuário inscreveu pode atualizar  uma extensão de esquema desde que a propriedade proprietária da extensão seja definida como **appId** de um aplicativo que o usuário de entrada possui. Esse aplicativo pode ser aquele que inicialmente criou a extensão ou algum outro aplicativo pertencente ao usuário in-locar. 

Esse critério para a propriedade **owner** permite que um usuário in-loco faça atualizações por meio de outros aplicativos que eles não têm, como o Microsoft Graph Explorer. Ao usar Graph Explorer para atualizar um recurso **schemaExtension,** inclua a propriedade **owner** no corpo da solicitação PATCH. Para obter mais informações, consulte a seção [Extensões](/graph/known-issues#extensions) em [Problemas conhecidos com a Microsoft Graph](/graph/known-issues).

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Application.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais

| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Content-Type   | application/json |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|description|String|Descrição da extensão de esquema.|
|properties|Coleção [extensionSchemaProperty](../resources/extensionschemaproperty.md)|A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema. Somente alterações aditiva são permitidas. |
|status|String|O estado do ciclo de vida da extensão do esquema. O estado inicial após a criação **é InDevelopment**. As transições de estados possíveis **são de InDevelopment** **para Disponível** e **Disponível** **para Preterido**.|
|targetTypes|Coleção de cadeias de caracteres|Conjunto de tipos Graph microsoft (que podem dar suporte a extensões) aos quais a extensão de esquema pode ser aplicada.  Somente alterações aditiva são permitidas.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



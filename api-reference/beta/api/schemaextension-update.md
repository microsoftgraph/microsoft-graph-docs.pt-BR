---
title: Update schemaExtension
description: Atualize as propriedades na definição da schemaExtension especificada.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 421a670c3d73caef5d5a4477233c36d202c44c6b
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352411"
---
# <a name="update-schemaextension"></a>Update schemaExtension

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades na definição da [schemaExtension](../resources/schemaextension.md)especificada. As atualizações aditivas para a extensão só poderão ser feitas quando a extensão estiver no **indevelopment** ou no status **disponível** . Isso significa que as propriedades personalizadas ou os tipos de recursos de destino não podem ser removidos da definição, mas novas propriedades personalizadas podem ser adicionadas e a descrição da extensão é alterada.

A atualização se aplica a todos os recursos incluídos na propriedade **TargetTypes** da extensão. Esses recursos estão entre os [tipos de recurso de suporte](/graph/extensibility-overview#supported-resources).

Para fluxos delegados, o usuário conectado pode atualizar uma extensão de esquema, desde que a propriedade **Owner** da extensão seja definida como a **AppID** de um aplicativo que o usuário conectado possui. Esse aplicativo pode ser aquele que criou inicialmente a extensão ou outro aplicativo pertencente ao usuário conectado. 

Esse critério para a propriedade **Owner** permite que um usuário conectado faça as atualizações por meio de outros aplicativos que não são de sua propriedade, como o Microsoft Graph Explorer. Ao usar o Graph Explorer para atualizar um recurso **schemaExtension** , inclua a propriedade **Owner** no corpo da solicitação patch. Para obter mais informações, consulte a seção [extensões](/graph/known-issues#extensions) em [problemas conhecidos com o Microsoft Graph](/graph/known-issues).

## <a name="permissions"></a>Permissões

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
|properties|Coleção [extensionSchemaProperty](../resources/extensionschemaproperty.md)|A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema. Somente as alterações aditivas são permitidas. |
|status|String|O estado do ciclo de vida da extensão do esquema. O estado inicial na criação é o **indevelopment**. Os possíveis transições de Estados estão de **indevelopment** para **Available** e **disponíveis** para **preteridos**.|
|targetTypes|Coleção de cadeias de caracteres|Conjunto de tipos do Microsoft Graph (que podem suportar extensões) à qual a extensão de esquema pode ser aplicada.  Somente as alterações aditivas são permitidas.|

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
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
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



---
title: Atualizar schemaExtension
description: Atualize as propriedades na definição da schemaExtension especificada.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: f457609af15716ef2ada3945132afd285fd2394c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515535"
---
# <a name="update-schemaextension"></a>Atualizar schemaExtension

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades na definição da [schemaExtension](../resources/schemaextension.md) especificada.

A atualização se aplica a todos os recursos que estão incluídos na propriedade **targetTypes** da extensão. Esses recursos estão entre os [tipos de recurso de suporte](/graph/extensibility-overview#supported-resources).

Somente o aplicativo que criou uma extensão de esquema (proprietário do aplicativo) pode fazer atualizações aditivas à extensão quando a extensão estiver com o status **InDevelopment** ou **Available**. Isso significa que o aplicativo não consegue remover propriedades personalizadas ou tipos de recursos de destino da definição. Porém, o aplicativo pode alterar a descrição da extensão.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
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
|status|String|O estado de ciclo de vida da extensão do esquema. O estado inicial após a criação é **InDevelopment**. Transições de estados possíveis vão de **InDevelopment** a **disponível** e **disponível** para **obsoleto**.|
|targetTypes|Coleção de cadeias de caracteres|O conjunto de tipos do Microsoft Graph (que podem suportar extensões) ao qual a extensão de esquema pode ser aplicada.  Somente as alterações aditivas são permitidas.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

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
  ],
}
```

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
    "Error: /api-reference/beta/api/schemaextension-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

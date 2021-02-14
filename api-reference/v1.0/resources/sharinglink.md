---
author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
description: O recurso SharingLink agrupa itens de dados relacionados ao link em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: def93edc26d90d40b480243431316c60a7f34e37
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239804"
---
# <a name="sharinglink-resource-type"></a>Tipo de recurso SharingLink

Namespace: microsoft.graph

O recurso **SharingLink** agrupa itens de dados relacionados ao link em uma única estrutura.

Se um recurso [**Permission**](permission.md) tiver uma faceta **sharingLink** não nula, a permissão representará um link de compartilhamento (em vez de permissões concedidas a uma pessoa ou um grupo).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": { "@odata.type": "microsoft.graph.identity" },
  "preventsDownload": false,
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo          | Descrição
|:------------|:--------------|:-------------------------------------
| aplicativo | [identity][]  | O aplicativo ao qual o link está associado.
| type        | Cadeia de caracteres        | O tipo do link criado.
| scope       | String        | O escopo do link representado por esta permissão. O valor `anonymous` indica que o link é utilizável por qualquer pessoa; `organization` indica que o link só é útil para usuários conectados ao mesmo locatário.
| preventsDownload | Booliano       | Se verdadeiro, o usuário só pode usar esse link para exibir o item na Web e não pode usá-lo para baixar o conteúdo do item. Somente para o OneDrive for Business e o SharePoint.
| webHtml     | String        | Para links `embed`, essa propriedade contém o código HTML para um elemento `<iframe>` que inserirá o item em uma página da Web.
| webUrl      | String        | Uma URL que abre o item no navegador no site do OneDrive.

[Identity]: identity.md

## <a name="type-options"></a>Opções de tipo

Esta tabela define os valores possíveis para a propriedade **type**:

| Valor   | Função    | Descrição
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | Um link somente de compartilhamento para exibição, permitindo o acesso somente leitura.
| `edit`  | `write` | Um link de compartilhamento de edição, permitindo o acesso de leitura e gravação.
| `embed` | `read`  | Um link de compartilhamento somente exibição que pode ser usado para inserir o conteúdo em uma página da Web de hospedagem. Os links de compartilhamento não estão disponíveis para OneDrive for Business ou SharePoint.

## <a name="scope-options"></a>Opções de escopo

| Valor          | Descrição
|:---------------|:------------------------------------------------------------
| `anonymous`    | Qualquer pessoa com o link tem acesso, sem precisar fazer logon. Isso pode incluir pessoas de fora da organização.
| `organization` | Qualquer pessoa que tenha feito logon em sua organização (locatário) pode usar o link para obter acesso. Disponível apenas no OneDrive for Business e no SharePoint.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(view,edit,embed) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization) are in resource, but () are in table"
  ],
  "tocPath": "Facets/SharingLink"
} -->


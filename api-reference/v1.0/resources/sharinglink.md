---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
ms.openlocfilehash: 7639dab9f63a948b3e9a849d8d320de60f5a0954
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2018
ms.locfileid: "23270486"
---
# <a name="sharinglink-resource-type"></a>Tipo de recurso SharingLink

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
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo          | Descrição
|:------------|:--------------|:-------------------------------------
| aplicativo | [identidade][]  | O aplicativo ao qual o link está associado.
| type        | Sequência de caracteres        | O tipo do link criado.
| scope       | Sequência de caracteres        | O escopo do link representado por esta permissão. O valor `anonymous` indica que o link é utilizável por qualquer pessoa; `organization` indica que o link só é útil para usuários conectados ao mesmo locatário.
| webHtml     | Sequência de caracteres        | Para links `embed`, essa propriedade contém o código HTML para um elemento `<iframe>` que inserirá o item em uma página da Web.
| webUrl      | Sequência de caracteres        | Uma URL que abre o item no navegador no site do OneDrive.

[Identidade]: identity.md

## <a name="type-options"></a>Opções de tipo

Esta tabela define os valores possíveis para a propriedade **type**:

| Valor   | Função    | Descrição
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | Um link somente de compartilhamento para exibição, permitindo o acesso somente leitura.
| `edit`  | `write` | Um link de compartilhamento de edição, permitindo o acesso de leitura e gravação.
| `embed` | `read`  | Um link de compartilhamento somente exibição que pode ser usado para inserir o conteúdo em uma página da Web de hospedagem. Links incorporados não estão disponíveis para OneDrive for Business ou SharePoint.

## <a name="scope-options"></a>Opções de escopo

| Valor          | Descrição
|:---------------|:------------------------------------------------------------
| `anonymous`    | Qualquer pessoa com o link possui acesso, sem precisar entrar. Isso pode incluir pessoas fora da sua organização.
| `organization` | Qualquer pessoa conectada na sua organização (locatário) pode usar o link para obter acesso. Disponível somente no OneDrive for Business e no SharePoint.

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

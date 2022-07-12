---
author: JeremyKelley
description: Os recursos sharingLink agrupam itens de dados relacionados ao link em uma única estrutura.
ms.date: 09/10/2017
title: SharingLink
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 27d9b586c0fe992075ee61424133e9b16259977c
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731908"
---
# <a name="sharinglink-resource-type"></a>Tipo de recurso sharingLink

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os **recursos sharingLink** agrupam itens de dados relacionados ao link em uma única estrutura.

Se um [**recurso**](permission.md) de permissão tiver uma faceta **sharingLink** não nula, a permissão representará um link de compartilhamento (em vez de permissões concedidas a uma pessoa ou grupo).

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

| Propriedade       | Tipo          | Descrição
|:---------------|:--------------|:-------------------------------------
| aplicativo    | [identity][]  | O aplicativo ao qual o link está associado.
| type           | String        | O tipo do link criado.
| scope          | String        | O escopo do link representado por esta permissão. O valor `anonymous` indica que o link é utilizável por qualquer pessoa; `organization` indica que o link só é útil para usuários conectados ao mesmo locatário.
| preventsDownload | Booliano       | Se for true, o usuário só poderá usar esse link para exibir o item na Web e não poderá usá-lo para baixar o conteúdo do item. Somente para OneDrive for Business e SharePoint.
| webHtml        | String        | Para links `embed`, essa propriedade contém o código HTML para um elemento `<iframe>` que inserirá o item em uma página da Web.
| webUrl         | String        | Uma URL que abre o item no navegador no site do OneDrive.

[Identity]: identity.md

### <a name="type-options"></a>Opções de tipo

A tabela a seguir define os valores possíveis para a **propriedade type** .

| Valor    | Role     | Descrição
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | Um link somente de compartilhamento para exibição, permitindo o acesso somente leitura.
| `edit`   | `write`  | Um link de compartilhamento de edição, permitindo o acesso de leitura e gravação.
| `embed`  | `read`   | Um link de compartilhamento somente exibição que pode ser usado para inserir o conteúdo em uma página da Web de hospedagem. Os links de compartilhamento não estão disponíveis para OneDrive for Business ou SharePoint.

### <a name="scope-options"></a>Opções de escopo

A tabela a seguir define os valores possíveis para a propriedade **de** escopo.

| Valor            | Descrição
|:-----------------|:------------------------------------------------------------
| `anonymous`      | Qualquer pessoa com o link tem acesso, sem precisar fazer logon. Isso pode incluir pessoas de fora da organização.
| `organization`   | Qualquer pessoa que tenha feito logon em sua organização (locatário) pode usar o link para obter acesso. Disponível apenas no OneDrive for Business e no SharePoint.
| `existingAccess` | Somente as pessoas que já tiverem acesso ao item por outros meios podem acessar o item usando este link. Disponível apenas no OneDrive for Business e no SharePoint.
| `users`          | O link concede acesso apenas a uma lista específica de pessoas. Disponível apenas no OneDrive for Business e no SharePoint.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



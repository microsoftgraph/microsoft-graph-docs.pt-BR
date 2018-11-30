---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
ms.openlocfilehash: 094de0cbdb77fe427ba70b9418ced5cc6e9cc731
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034797"
---
# <a name="sharinglink-resource-type"></a>tipo de recurso de sharingLink

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso de **sharingLink** agrupa itens de dados relacionados à link em uma única estrutura.

Se um recurso de [**permissão**](permission.md) tiver uma faceta não nulas **sharingLink** , a permissão representa um link de compartilhamento (ao contrário de permissões concedidas para uma pessoa ou grupo).

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
| preventsDownload | Booliano       | Se for true, em seguida, o usuário só pode usar este link para exibir o item na web e não pode ser usado para baixar o conteúdo do item. Somente para OneDrive for Business e o SharePoint.
| webHtml        | String        | Para links `embed`, essa propriedade contém o código HTML para um elemento `<iframe>` que inserirá o item em uma página da Web.
| webUrl         | String        | Uma URL que abre o item no navegador no site do OneDrive.

[Identity]: identity.md

### <a name="type-options"></a>Opções de tipo

A tabela a seguir define os valores possíveis para a propriedade **type** .

| Valor    | Função     | Descrição
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | Um link somente de compartilhamento para exibição, permitindo o acesso somente leitura.
| `edit`   | `write`  | Um link de compartilhamento de edição, permitindo o acesso de leitura e gravação.
| `embed`  | `read`   | Um link de compartilhamento somente exibição que pode ser usado para inserir o conteúdo em uma página da Web de hospedagem. Os links de compartilhamento não estão disponíveis para OneDrive for Business ou SharePoint.

### <a name="scope-options"></a>Opções de escopo

A tabela a seguir define os valores possíveis para a propriedade de **escopo** .

| Valor            | Descrição
|:-----------------|:------------------------------------------------------------
| `anonymous`      | Qualquer pessoa com o link possui acesso, sem precisar entrar. Isso pode incluir pessoas fora da sua organização.
| `organization`   | Qualquer pessoa entrado na sua organização (inquilino) pode usar o link para obter acesso. Disponível somente no OneDrive for Business e o SharePoint.
| `existingAccess` | Somente as pessoas que já tiverem sido concedidas acesso ao item por outros meios podem acessar o item usando este link. Disponível somente no OneDrive for Business e o SharePoint.
| `users`          | O link concede acesso somente a uma lista específica de pessoas. Disponível somente no OneDrive for Business e o SharePoint.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": ""
}-->

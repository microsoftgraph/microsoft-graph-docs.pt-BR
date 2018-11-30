---
title: Tipo de recurso openTypeExtension (extensões abertas)
description: Extensões de Open (conhecidas anteriormente como extensões de dados do Office 365) fornecem uma maneira fácil de adicionar diretamente sem tipo propriedades para um recurso no Microsoft Graph.
ms.openlocfilehash: eedf61ccdda62ab69673a4489b49db782f514ef0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004507"
---
# <a name="opentypeextension-resource-type-open-extensions"></a>Tipo de recurso openTypeExtension (extensões abertas)

Extensões de Open (conhecidas anteriormente como extensões de dados do Office 365) fornecem uma maneira fácil de adicionar diretamente sem tipo propriedades para um recurso no Microsoft Graph.

Extensões abertas são representadas pelo recurso **openTypeExtension**. Qualquer extensão aberta adicionada a um recurso é mostrada na propriedade de navegação **extensions**, que deriva do tipo abstrato [extension](extension.md). Cada extensão tem uma propriedade **extensionName**, que é a única propriedade predefinida e gravável para todas as extensões, juntamente com seus dados personalizados.

Um modo de garantir que os nomes de extensão sejam exclusivos é usar um formato reverso de DNS no sistema de nomes de domínio que dependa de _seu próprio domínio_, por exemplo, `Com.Contoso.ContactInfo`. Não use o domínio Microsoft (`Com.Microsoft` ou `Com.OnMicrosoft`) em um nome de extensão.

Exemplo de extensão aberta: [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)

As extensões abertas têm suporte nos recursos a seguir nas versões correspondentes - disponibilidade geral (GA: /v1.0 e /beta) ou visualização (/beta).

|Recurso |Versão |
|:---------------|:-------|
| [Unidade administrativa](/graph/api/resources/administrativeunit?view=graph-rest-beta)  | Somente para visualização |
| [Evento de calendário](event.md) | GA |
| [Evento de calendário](event.md) do grupo | GA |
| [Postagem](post.md) de thread de conversa do grupo | GA |
| [device](device.md) | GA |
| [group](group.md) | GA |
| [message](message.md) | GA |
| [organization](organization.md) | GA |
| [Contato pessoal](contact.md) | GA |
| [user](user.md) | GA |

## <a name="outlook-specific-considerations"></a>Considerações específicas do Outlook

Cada extensão aberta presente em um recurso do Outlook (evento, mensagem ou contato pessoal) é armazenado em uma [propriedade MAPI nomeada](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx). Quando você cria extensões abertas para o Outlook, considere que o MAPI denominada propriedades sejam um recurso finito na caixa de correio do usuário. Quando for esgotada cota do nome da propriedade de um usuário, é possível criar qualquer propriedades nomeadas mais para esse usuário. Isso pode resultar em um comportamento inesperado de clientes que dependem de propriedades nomeadas funcione.

Aplique as seguintes diretrizes ao criar extensões open nos recursos do Outlook:

- Crie o número mínimo de extensões necessárias. A maioria dos aplicativos deve exigir que não mais de uma extensão. As extensões não têm propriedades de conjunto definido ou estrutura, permitindo que você armazene vários valores em um única extensão.
- Evite extensões de nomes de maneira variável (como com base na entrada do usuário, etc.). Cada vez que uma extensão aberta é criada com um novo nome não tiver sido usado na caixa de correio de um usuário antes, um novo MAPI denominado propriedade é criado. Removendo a extensão não remove a propriedade nomeada.

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>Usar extensões open (para recursos do Outlook) ou propriedades estendidas

Extensões Open são a solução recomendada para a maioria dos cenários que envolvem armazenar e acessar dados personalizados. Se, no entanto, você precisar acessar dados personalizados para propriedades MAPI do Outlook que não são expostos por meio de [metadados de API do Microsoft Graph](https://developer.microsoft.com/graph/docs/overview/call_api), você pode usar [propriedades estendidas e seus API REST](extended-properties-overview.md). Você pode verificar quais propriedades os metadados expõe em [ https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.extension",
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a>Propriedades

|Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|extensionName|String|Um identificador de texto exclusivo para uma extensão de tipo aberto. Obrigatório.|
|id|String| Um identificador totalmente qualificado que concatena o tipo de extensão com **extensionName**. Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="methods"></a>Métodos

|Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Post](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md) (em uma instância de recurso existente) ou um novo [contact](../resources/contact.md), [event](../resources/event.md) ou [message](../resources/message.md) que contenha um objeto openTypeExtension | Crie um objeto openTypeExtension em uma instância de recurso nova ou existente.|
|[Get](../api/opentypeextension-get.md) | [openTypeExtension](opentypeextension.md) |Leia propriedades e relações do objeto openTypeExtension.|
|[Update](../api/opentypeextension-update.md) | [openTypeExtension](opentypeextension.md) |Atualize o objeto openTypeExtension. |
|[Delete](../api/opentypeextension-delete.md) | Nenhuma |Exclua um objeto openTypeExtension. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

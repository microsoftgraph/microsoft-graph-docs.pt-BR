---
title: Tipo de recurso openTypeExtension (extensões abertas)
description: As extensões abertas (anteriormente conhecidas como extensões de dados do Office 365) oferecem uma maneira fácil de adicionar diretamente propriedades não tipadas a um recurso do Microsoft Graph.
ms.localizationpriority: medium
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: 57d1af2db82f47be3a3f6faf11768ff2ccf89933
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555469"
---
# <a name="opentypeextension-resource-type-open-extensions"></a>Tipo de recurso openTypeExtension (extensões abertas)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi-sharedfeature](../includes/todo-deprecate-basetaskapi-sharedfeature.md)]

Representa extensões abertas (anteriormente conhecidas como extensões de dados Office 365), uma opção de [extensibilidade](/graph/extensibility-overview) que fornece uma maneira fácil de adicionar propriedades não tipadas diretamente a um recurso no Microsoft Graph.

Qualquer extensão aberta adicionada a um recurso aparece na propriedade **de navegação de** extensões. Cada extensão tem uma propriedade **extensionName**, que é a única propriedade predefinida e gravável para todas as extensões, juntamente com seus dados personalizados. Um modo de garantir que os nomes de extensão sejam exclusivos é usar um formato reverso de DNS no sistema de nomes de domínio que dependa de _seu próprio domínio_, por exemplo, `com.contoso.ContactInfo`. **Não use o** domínio da Microsoft (`com.microsoft` ou `com.onmicrosoft`) em um nome de extensão.

Deriva do tipo [abstrato de](extension.md) extensão.

As extensões abertas são compatíveis com os recursos a seguir.

+ [user](/graph/api/resources/user)
+ [group](/graph/api/resources/group)
<!--+ [administrativeUnit](/graph/api/resources/administrativeunit)-->
+ [contact](/graph/api/resources/contact)
+ [device](/graph/api/resources/device)
+ [evento](/graph/api/resources/event) para calendários de usuário e grupo
+ [message](/graph/api/resources/message)
+ [organização](/graph/api/resources/organization)
+ [postagem](/graph/api/resources/post)
+ [todoTask](todotask.md) 
+ [todoTaskList](todotasklist.md)
+ [baseTaskList](basetasklist.md) (preterido)
+ [baseTask](basetask.md) (preterido)

> **Nota:** \* Devido a uma limitação de serviço existente, os representantes não podem criar eventos abertos acrescentados à extensão em calendários de caixa de correio compartilhados. As tentativas de fazer isso resultarão em uma resposta de `ErrorAccessDenied`.

Para obter mais informações sobre a extensibilidade do Microsoft Graph, incluindo limites para extensões abertas, consulte Adicionar propriedades personalizadas aos recursos usando extensões e Adicionar dados personalizados aos usuários usando [extensões abertas](/graph/extensibility-open-users).[](/graph/extensibility-overview)

### <a name="outlook-specific-considerations"></a>Considerações específicas do Outlook

Cada extensão aberta presente em um recurso do Outlook (evento, mensagem ou contato pessoal) é armazenada em uma [propriedade MAPI](/office/client-developer/outlook/mapi/mapi-named-properties). Quando você cria extensões abertas no Outlook, considere que as propriedades MAPI são um recurso finito em uma caixa de correio do usuário. Quando a propriedade de cota de um usuário acabar, não será mais possível criar quaisquer propriedades nomeadas desse usuário. Isso pode resultar em um comportamento inesperado de clientes que dependem de propriedades nomeadas para funcionar.

Aplique as seguintes diretrizes quando você criar extensões abertas em recursos do Outlook:

- Crie um número mínimo de extensões necessárias. A maioria dos aplicativos exigem não mais que uma extensão. As extensões não têm um conjunto definido de propriedades nomeadas ou estrutura, para que seja possível armazenar vários valores em um única extensão.
- Evite renomear extensões de uma maneira variável (por exemplo, com base na entrada do usuário, etc.). Sempre que uma extensão aberta é criada com um novo nome que não foi usado na caixa de correio do usuário, uma nova propriedade MAPI é criada. Remover a extensão não remove a propriedade nomeada.

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>Use extensões abertas (para recursos do Outlook) ou propriedades estendidas

As extensões abertas são a solução recomendada para a maioria dos cenários que envolvem armazenar e acessar dados personalizados. Se, no entanto, você precisar acessar dados personalizados para as propriedades do Outlook MAPI que já não estão expostos por meio dos [metadados da API do Microsoft Graph](/graph/traverse-the-graph#microsoft-graph-api-metadata), você pode usar as [propriedades estendidas e sua API REST](extended-properties-overview.md). Você pode confirmar quais propriedades os metadados expõem em https://graph.microsoft.com/v1.0/$metadata.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Criar](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md) (em uma instância de recurso existente) ou um novo [contato baseTask](basetask.md), [baseTaskList](basetasklist.md)[,](contact.md) [evento](event.md)[, mensagem](message.md), [post](post.md), [todoTask](todotask.md) [ou todoTaskList](todotasklist.md) que contém um objeto openTypeExtension. | Crie um objeto openTypeExtension em uma instância de recurso nova ou existente.|
|[Get](../api/opentypeextension-get.md) | [openTypeExtension](opentypeextension.md) |Leia propriedades e relações do objeto openTypeExtension.|
|[Update](../api/opentypeextension-update.md) | [openTypeExtension](opentypeextension.md) |Atualize o objeto openTypeExtension. |
|[Delete](../api/opentypeextension-delete.md) | Nenhuma |Exclua um objeto openTypeExtension. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|extensionName|String|Um identificador de texto exclusivo para uma extensão de dados de tipo aberto. Obrigatório.|
|id|String| Um identificador totalmente qualificado que concatena o tipo de extensão com **extensionName**. Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}
```

## <a name="see-also"></a>Confira também

+ [Adicionar propriedades personalizadas a recursos usando extensões](/graph/extensibility-overview)
+ [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

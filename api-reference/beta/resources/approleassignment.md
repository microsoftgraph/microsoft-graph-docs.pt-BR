---
title: tipo de recurso de appRoleAssignment
description: Usado para registrar quando um usuário ou grupo for atribuído a um aplicativo. Nesse caso, a atribuição de função resultará em um elemento de aplicativo aparecendo backup na painel de acesso do aplicativo do usuário. Esta entidade também pode ser usada para conceder acesso de outro aplicativo (modelado como uma entidade de serviço) para um aplicativo de recursos em uma determinada função. Você pode criar, ler, atualizar e excluir atribuições de função.
localization_priority: Priority
ms.openlocfilehash: 3276c1f34b91dc628ed00f2ffbc64ffe56899bdf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845469"
---
# <a name="approleassignment-resource-type"></a>tipo de recurso de appRoleAssignment

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Usado para registrar quando um usuário ou grupo for atribuído a um aplicativo. Nesse caso, a atribuição de função resultará em um elemento de aplicativo aparecendo backup na painel de acesso do aplicativo do usuário. Esta entidade também pode ser usada para conceder acesso de outro aplicativo (modelado como uma entidade de serviço) para um aplicativo de recursos em uma determinada função. Você pode criar, ler, atualizar e excluir atribuições de função.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approleassignment"
}-->

```json
{
  "creationTimestamp": "String (timestamp)",
  "id": "guid (identifier)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|creationTimestamp|DateTimeOffset|A hora em que a concessão foi criada. O tipo de carimbo de hora representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|Guid|A id de função que foi atribuída à entidade de segurança.  Essa função deve ser declarada pelo destino recurso aplicativo **resourceId** em sua propriedade **appRoles** . Onde o recurso não declarar todas as permissões, uma id do padrão (zero GUID) deve ser especificada. Chave. Não anulável. |
|principalDisplayName|Cadeia de caracteres|O nome de exibição da entidade que foi concedido o acesso.|
|principalId|Guid|O identificador exclusivo (**id**) para a entidade sendo concedida o acesso. Necessários na criação.            |
|principalType|Cadeia de caracteres|O tipo de entidade.  Isso pode ser "User", "Grupo" ou "ServicePrincipal".|
|resourceDisplayName|Cadeia de caracteres|O nome de exibição do recurso para o qual a atribuição foi feita.|
|resourceId|Guid|O identificador exclusivo (**id**) para o recurso de destino (entidade de serviço) para o qual a atribuição foi feita.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter appRoleAssignment](../api/approleassignment-get.md) | [appRoleAssignment](approleassignment.md) |Leia as propriedades e os relacionamentos do objeto appRoleAssignment.|
|[Update](../api/approleassignment-update.md) | [appRoleAssignment](approleassignment.md)   |Atualize o objeto appRoleAssignment. |
|[Delete](../api/approleassignment-delete.md) | Nenhum |Exclua objeto appRoleAssignment. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

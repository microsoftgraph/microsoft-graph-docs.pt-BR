---
title: Tipo de recurso externalGroup
description: Representa um grupo externo usado para definir permissões em externalItems adicionados a uma conexão do Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 2e9d8e3a605f1c3df39b13607f82e7541d59e62e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161697"
---
# <a name="externalgroup-resource-type"></a>Tipo de recurso externalGroup

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um grupo externo. Grupos externos (juntamente com usuários e grupos do Azure Active Directory) são usados para definir permissões em **externalItems adicionados** a uma conexão do Microsoft Graph. Use **externalGroups** para representar grupos do Active Directory não Azure ou construções do tipo grupo (como unidades de negócios, Teams e es) que determinam a permissão sobre o conteúdo em sua fonte de dados externa.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar externalGroup](../api/externalconnection-post-groups.md)|[externalGroup](../resources/externalgroup.md)|Criar um novo **objeto externalGroup.**|
|[Excluir externalGroup](../api/externalgroup-delete.md)|Nenhum(a)|**Exclua um objeto externalGroup.**|
|[Criar membros](../api/externalgroup-post-members.md)|[externalGroupMember](../resources/externalgroupmember.md)|Criar um novo **objeto externalGroupMember.**|

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo   | Descrição                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | String | A ID exclusiva do grupo externo dentro de uma conexão. Ele deve ser alfanumérico e ter até 128 caracteres. |
| displayName | String | O nome amigável do grupo externo. Opcional.                                                                       |
| description | String | A descrição do grupo externo. Opcional.                                                                         

## <a name="relationships"></a>Relações

| Relação | Tipo                                                                  | Descrição                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| membros      | [Coleção externalGroupMember](../resources/externalgroupmember.md) | Um membro adicionado a um **externalGroup**. Você pode adicionar usuários do Azure Active Directory, grupos do Azure Active Directory ou outros **grupos externos como** membros. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroup",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```

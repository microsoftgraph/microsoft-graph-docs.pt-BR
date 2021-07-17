---
title: Tipo de recurso externalGroup
description: Representa um grupo externo usado para definir permissões em externalItems adicionados a uma conexão Graph Microsoft.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3f0c6adbd47d1823b82e19d3fb9a352e26391da9
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467570"
---
# <a name="externalgroup-resource-type"></a>Tipo de recurso externalGroup

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um grupo externo. Grupos externos (juntamente com Azure Active Directory e grupos) são usados para definir permissões em **externalItems adicionados** a uma conexão microsoft Graph. Use **externalGroups** para representar grupos não Azure Active Directory ou construções do tipo grupo (como unidades de negócios, Teams e filho on) que determinam a permissão sobre o conteúdo em sua fonte de dados externa.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar externalGroup](../api/externalconnectors-externalconnection-post-groups.md)|[microsoft.graph.externalConnectors.externalGroup](../resources/externalconnectors-externalgroup.md)|Crie um novo **objeto externalGroup.**|
|[Excluir externalGroup](../api/externalconnectors-externalgroup-delete.md)|Nenhum|**Exclua um objeto externalGroup.**|
|[Criar membros](../api/externalconnectors-externalgroup-post-members.md)|[microsoft.graph.externalConnectors.externalGroupMember](../resources/externalconnectors-externalgroupmember.md)|Crie um novo **objeto externalGroupMember.**|

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo   | Descrição                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | String | A ID exclusiva do grupo externo dentro de uma conexão. Ele deve ser alfanumérico e pode ter até 128 caracteres. |
| displayName | String | O nome amigável do grupo externo. Opcional.                                                                       |
| description | String | A descrição do grupo externo. Opcional.                                                                         

## <a name="relationships"></a>Relações

| Relação | Tipo                                                                  | Descrição                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| membros      | [Coleção microsoft.graph.externalConnectors.externalGroupMember](../resources/externalconnectors-externalgroupmember.md) | Um membro adicionado a **um externalGroup**. Você pode adicionar Azure Active Directory usuários, Azure Active Directory grupos ou outros **externalGroups** como membros. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```

---
title: Tipo de recurso externalGroup
description: Representa um grupo que não Azure Active Directory grupo.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5fbfcb8b462b490b33519f04268c505871613a24
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697384"
---
# <a name="externalgroup-resource-type"></a>Tipo de recurso externalGroup

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Namespace: microsoft.graph.externalConnectors

Representa um grupo que não Azure Active Directory grupo.

Grupos externos determinam permissões para o conteúdo em sua fonte de dados externa. Esses grupos externos podem ser usados em entradas na [acl](../resources/externalconnectors-externalitem.md) de [um externalItem](../resources/externalconnectors-externalitem.md).

Exemplos de grupos externos são unidades de negócios e equipes de trabalho.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar externalGroup](../api/externalconnectors-externalconnection-post-groups.md)|[microsoft.graph.externalConnectors.externalGroup](../resources/externalconnectors-externalgroup.md)|Crie um novo **objeto externalGroup.**|
|[Excluir externalGroup](../api/externalconnectors-externalgroup-delete.md)|Nenhum|**Exclua um objeto externalGroup.**|
|[Criar membro](../api/externalconnectors-externalgroup-post-members.md)|[microsoft.graph.externalConnectors.externalGroupMember](../resources/externalconnectors-externalgroupmember.md)|Crie um novo **objeto externalGroupMember.**|

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo   | Descrição                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | Cadeia de caracteres | A ID exclusiva do grupo externo dentro de uma conexão. Ele deve ser alfanumérico e pode ter até 128 caracteres. |
| displayName | Cadeia de caracteres | O nome amigável do grupo externo. Opcional.                                                                       |
| descrição | Cadeia de caracteres | A descrição do grupo externo. Opcional.                                                                         

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

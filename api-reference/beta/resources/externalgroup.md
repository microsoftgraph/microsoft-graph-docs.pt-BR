---
title: tipo de recurso de interexternal
description: Representa um grupo externo usado para definir permissões no externalItems adicionado a uma conexão do Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c258df9e6f20cf7a19e291fd298ad66345a72949
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193811"
---
# <a name="externalgroup-resource-type"></a>tipo de recurso de interexternal

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um grupo externo. Grupos externos (juntamente com usuários e grupos do Azure Active Directory) são usados para definir permissões no **externalItems** adicionado a uma conexão do Microsoft Graph. Use o **externalGroups** para representar grupos do Active Directory do Azure ou construções do tipo grupo (como unidades de negócios, equipes e filho) que determinam a permissão sobre o conteúdo da sua fonte de dados externa.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar um](../api/externalconnection-post-groups.md)|[externa](../resources/externalgroup.md)|Criar um novo objeto de objeto **externo** .|
|[Excluir o external](../api/externalgroup-delete.md)|Nenhum|Excluir um **objeto** de um.|
|[Criar membros](../api/externalgroup-post-members.md)|[externalGroupMember](../resources/externalgroupmember.md)|Criar um novo objeto **externalGroupMember** .|

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo   | Descrição                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | String | A identificação exclusiva do grupo externo em uma conexão. Ele deve ser alfanumérico e até 128 caracteres de comprimento. |
| displayName | String | O nome amigável do grupo externo. Opcional.                                                                       |
| description | String | A descrição do grupo externo. Opcional.                                                                         

## <a name="relationships"></a>Relações

| Relação | Tipo                                                                  | Descrição                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| membros      | coleção [externalGroupMember](../resources/externalgroupmember.md) | Um membro adicionado a uma **myexterna**. Você pode adicionar usuários do Azure Active Directory, grupos do Azure Active Directory ou outros **externalGroups** como membros. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroup",
  "baseType": "",
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

---
title: Tipo de recurso externalGroup
description: Representa um grupo que não Azure Active Directory grupo.
author: sacampbe-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 2f944032cbe58972ecab1075ca01053817f9de63
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697486"
---
# <a name="externalgroup-resource-type"></a>Tipo de recurso externalGroup

Namespace: microsoft.graph.externalConnectors

Representa um grupo que não Azure Active Directory grupo.

Grupos externos determinam permissões para o conteúdo em sua fonte de dados externa. Esses grupos externos podem ser usados em entradas na [acl](../resources/externalconnectors-externalitem.md) de [um externalItem](../resources/externalconnectors-externalitem.md).

Exemplos de grupos externos são unidades de negócios e equipes de trabalho.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar externalGroup](../api/externalconnectors-externalconnection-post-groups.md)|[microsoft.graph.externalConnectors.externalGroup](../resources/externalconnectors-externalgroup.md)|Crie um novo **objeto externalGroup.**|
|[Obter externalGroup](../api/externalconnectors-externalgroup-get.md)|[microsoft.graph.externalConnectors.externalGroup](../resources/externalconnectors-externalgroup.md)|Obter um **objeto externalGroup.**|
|[Atualizar externalGroup](../api/externalconnectors-externalgroup-update.md)|[microsoft.graph.externalConnectors.externalGroup](../resources/externalconnectors-externalgroup.md)|Atualize as propriedades de um **objeto externalGroup.**|
|[Excluir externalGroup](../api/externalconnectors-externalgroup-delete.md)|Nenhum|**Exclua um objeto externalGroup.**|

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo   | Descrição                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | Cadeia de caracteres | A ID exclusiva do grupo externo dentro de uma conexão. Ele deve ser alfanumérico e pode ter até 128 caracteres. |
| displayName | Cadeia de caracteres | O nome amigável do grupo externo. Opcional.                                                                       |
| descrição | Cadeia de caracteres | A descrição do grupo externo. Opcional.        

## <a name="relationships"></a>Relações

| Relação | Tipo                                                                  | Descrição                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| membros      | [coleção microsoft.graph.externalConnectors.identity](../resources/externalconnectors-identity.md) | Um membro adicionado a **um externalGroup**. Você pode adicionar Azure Active Directory usuários, Azure Active Directory grupos ou **um externalGroup** como membros. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup",
  "baseType": "microsoft.graph.entity",
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

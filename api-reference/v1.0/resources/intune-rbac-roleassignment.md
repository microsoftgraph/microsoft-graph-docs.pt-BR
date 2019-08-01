---
title: Tipo de recurso roleAssignment
description: O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 542cd188653465f2482e4a5fe837eeb811fe3bd6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037125"
---
# <a name="roleassignment-resource-type"></a>Tipo de recurso roleAssignment

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar roleAssignments](../api/intune-rbac-roleassignment-list.md)|Conjunto [roleAssignment](../resources/intune-rbac-roleassignment.md)|Listar propriedades e relações de objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|[Obter roleAssignment](../api/intune-rbac-roleassignment-get.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|Ler propriedades e relações de objetos de [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|[Create roleAssignment](../api/intune-rbac-roleassignment-create.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|Criar um novo objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|[Excluir roleAssignment](../api/intune-rbac-roleassignment-delete.md)|Nenhum|Excluir [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|[Atualizar roleAssignment](../api/intune-rbac-roleassignment-update.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|Atualizar as propriedades de um objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. É somente leitura e gerada automaticamente.|
|displayName|Cadeia de caracteres|O nome de exibição ou nome amigável da atribuição de função.|
|descrição|String|Descrição da atribuição de função.|
|resourceScopes|Coleção de cadeias de caracteres|Lista de IDs de grupos de segurança de membros de escopo da função.  Estas são as IDs do Azure Active Directory.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune-rbac-roledefinition.md)|A definição de função da qual essa atribuição faz parte.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ]
}
```




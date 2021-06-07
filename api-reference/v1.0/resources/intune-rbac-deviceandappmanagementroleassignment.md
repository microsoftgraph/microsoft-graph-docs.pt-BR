---
title: Tipo de recurso deviceAndAppManagementRoleAssignment
description: O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9c327790cd34b123e32fd0ad5d96039b22b804b7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752291"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a>Tipo de recurso deviceAndAppManagementRoleAssignment

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas.


Herda de [roleAssignment](../resources/intune-rbac-roleassignment.md)

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceAndAppManagementRoleAssignments](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|Coleção [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Lista propriedades e relações dos objetos [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).|
|[Obter deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Propriedades de leitura e relações do objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).|
|[Criar deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Cria um novo objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).|
|[Excluir deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|Nenhum|Exclui um [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).|
|[Atualizar deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Atualiza as propriedades de um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. É somente leitura e gerada automaticamente. Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|displayName|Cadeia de caracteres|O nome de exibição ou nome amigável da atribuição de função. Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|descrição|Cadeia de caracteres|Descrição da atribuição de função. Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|resourceScopes|Coleção de cadeias de caracteres|Lista de IDs de grupos de segurança de membros de escopo da função.  Estas são as IDs do Azure Active Directory. Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|members|Coleção de cadeias de caracteres|A lista de IDs de grupos de segurança de membros da função. Estas são as IDs do Azure Active Directory.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune-rbac-roledefinition.md)|A definição de função da qual essa atribuição faz parte. Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```





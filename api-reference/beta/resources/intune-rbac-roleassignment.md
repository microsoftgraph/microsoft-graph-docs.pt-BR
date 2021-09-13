---
title: Tipo de recurso roleAssignment
description: O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b7cb484ca45052fc6361c620022b2d166f7ec9db
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020284"
---
# <a name="roleassignment-resource-type"></a>Tipo de recurso roleAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
|id|String|Chave da entidade. É somente leitura e gerada automaticamente.|
|displayName|String|O nome de exibição ou nome amigável da atribuição de função.|
|description|Cadeia de caracteres|Descrição da atribuição de função.|
|scopeMembers|Coleção de cadeias de caracteres|Lista de IDs de grupos de segurança de membros de escopo da função.  Estas são as IDs do Azure Active Directory.|
|scopeType|[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)|Especifica o tipo de escopo de uma atribuição de função. O tipo padrão 'ResourceScope' permite a atribuição de ResourceScopes. Para 'AllDevices', 'AllLicensedUsers' e 'AllDevicesAndLicensedUsers', a propriedade ResourceScopes deve ser deixada vazia. Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.|
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
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ]
}
```




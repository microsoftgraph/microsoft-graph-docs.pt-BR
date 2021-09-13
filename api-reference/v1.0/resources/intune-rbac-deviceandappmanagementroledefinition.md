---
title: Tipo de recurso deviceAndAppManagementRoleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c956cdd086f95a682563d7039826e323c267ab36
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59028889"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a>Tipo de recurso deviceAndAppManagementRoleDefinition

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.


Herda de [roleDefinition](../resources/intune-rbac-roledefinition.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceAndAppManagementRoleDefinitions](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|Coleção [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).|
|[Obter deviceAndAppManagementRoleDefinition](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|Propriedades de leitura e relações do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).|
|[Criar deviceAndAppManagementRoleDefinition](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).|
|[Excluir deviceAndAppManagementRoleDefinition](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|Nenhum|Exclui um [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).|
|[Atualizar deviceAndAppManagementRoleDefinition](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|Atualiza as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. É somente leitura e gerada automaticamente. Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)|
|displayName|String|Nome de exibição da definição de Função. Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)|
|description|Cadeia de caracteres|Descrição da definição de Função. Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)|
|rolePermissions|Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)|Lista de Permissões de Função que esta função está autorizada a executar. Elas devem corresponder ao actionName definido como parte de rolePermission. Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)|
|isBuiltIn|Booliano|Tipo de Função. Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada. Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|roleAssignments|Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)|Lista de atribuições de função para esta definição de função. Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```





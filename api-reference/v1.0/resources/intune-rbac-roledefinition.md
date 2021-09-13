---
title: Tipo de recurso roleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7516a95a0da4d58b4604bbafa18132280e6a2ad1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126790"
---
# <a name="roledefinition-resource-type"></a>Tipo de recurso roleDefinition

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar roleDefinitions](../api/intune-rbac-roledefinition-list.md)|Coleção [roleDefinition](../resources/intune-rbac-roledefinition.md)|Listar propriedades e relações dos objetos [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|[Obter roleDefinition](../api/intune-rbac-roledefinition-get.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md)|Ler propriedades e relações do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|[Criar roleDefinition](../api/intune-rbac-roledefinition-create.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md)|Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)|
|[Excluir roleDefinition](../api/intune-rbac-roledefinition-delete.md)|Nenhum|Excluir um [roleDefinition](../resources/intune-rbac-roledefinition.md)|
|[Atualizar roleDefinition](../api/intune-rbac-roledefinition-update.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md)|Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. É somente leitura e gerada automaticamente.|
|displayName|String|Nome de exibição da definição de Função.|
|description|Cadeia de caracteres|Descrição da definição de Função.|
|rolePermissions|Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)|Lista de Permissões de Função que esta função está autorizada a executar. Elas devem corresponder ao actionName definido como parte de rolePermission.|
|isBuiltIn|Booliano|Tipo de Função. Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|roleAssignments|Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)|Lista de atribuições de função para esta definição de função.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
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





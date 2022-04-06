---
title: Tipo de recurso educationClass
description: 'Representa uma aula em uma escola. O **recurso educationClass** corresponde ao grupo Microsoft 365 e compartilha a mesma ID. Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados. Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.  '
ms.localizationpriority: medium
author: mlafleur
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e3b3a8618342afd21f9d18cc1d1c96fa2ed9bbf9
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685240"
---
# <a name="educationclass-resource-type"></a>Tipo de recurso educationClass

Namespace: microsoft.graph

Representa uma aula em uma escola. O **recurso educationClass** corresponde ao grupo Microsoft 365 e compartilha a mesma ID. Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados. Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods

| Método                                                   | Tipo de retorno                                                 | Descrição                                                                                          |
| :------------------------------------------------------- | :---------------------------------------------------------- | :--------------------------------------------------------------------------------------------------- |
| [Listar educationClasses](../api/educationclass-list.md)   | Coleção [educationClass](../resources/educationclass.md) | Obtenha uma lista dos [objetos educationClass](../resources/educationclass.md) e suas propriedades.     |
| [Criar educationClass](../api/educationclass-post.md) | [educationClass](../resources/educationclass.md)            | Crie um novo [objeto educationClass](../resources/educationclass.md) .                                |
| [Obter educationClass](../api/educationclass-get.md)       | [educationClass](../resources/educationclass.md)            | Leia as propriedades e as relações de um [objeto educationClass](../resources/educationclass.md) . |
| [Atualizar educationClass](../api/educationclass-update.md) | [educationClass](../resources/educationclass.md)            | Atualize as propriedades de um [objeto educationClass](../resources/educationclass.md) .                 |
| [Excluir educationClass](../api/educationclass-delete.md) | Nenhuma                                                        | Exclua [um objeto educationClass](../resources/educationclass.md) .                                  |
| [delta](../api/educationclass-delta.md)                  | Coleção [educationClass](../resources/educationclass.md) | Obter alterações incrementais na coleção de recursos.                                                  |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                           | Descrição                                                        |
| :------------------- | :--------------------------------------------- | :----------------------------------------------------------------- |
| id                   | Cadeia de caracteres                                         | Identificador de objeto. Herdado da [entidade](../resources/entity.md). |
| displayName          | Cadeia de caracteres                                         | Nome da aula.                                                 |
| mailNickname         | String                                         | Nome de email para enviar email a todos os membros, se essa propriedade estiver habilitada.    |
| description          | Cadeia de caracteres                                         | Descrição da aula.                                          |
| createdBy            | [identitySet](../resources/identityset.md)     | Entidade que criou a aula                                       |
| classCode            | Cadeia de caracteres                                         | Código de aula usada pela escola para identificar a aula.               |
| externalName         | Cadeia de caracteres                                         | Nome da aula no sistema de sincronização.                           |
| externalId           | Cadeia de caracteres                                         | ID da aula no sistema de sincronização.                           |
| externalSource       | educationExternalSource                        | Como essa aula foi criada. Os valores possíveis são: `sis` e `manual`.  |
| externalSourceDetail | Cadeia de caracteres                                         | O nome da fonte externa da qual esses recursos foram gerados. |
| grade                | Cadeia de caracteres                                         | Nível de nota da classe.                                          |
| term                 | [educationTerm](../resources/educationterm.md) | Termos dessa aula.                                               |

## <a name="relationships"></a>Relações

| Relação | Tipo                                                          | Descrição                                               |
| :----------- | :------------------------------------------------------------ | :-------------------------------------------------------- |
| assignments  | [coleção educationAssignment](educationAssignment.md) | Todas as atribuições associadas a essa classe. Anulável.     |
| group        | [group](../resources/group.md)                                | O objeto Microsoft 365 grupo subjacente.                |
| members      | Coleção [educationUser](../resources/educationuser.md)     | Todos os usuários da aula. Anulável.                         |
| schools      | Coleção [educationSchool](../resources/educationschool.md) | Todas as escolas às quais essa aula está associada. Anulável. |
| teachers     | Coleção [educationUser](../resources/educationuser.md)     | Todos os professores da aula. Anulável.                      |
|assignmentCategories| [coleção educationCategory](educationcategory.md) | Todas as categorias associadas a essa classe. Anulável. |
|assignmentDefaults| [coleção educationAssignmentDefaults](educationassignmentdefaults.md) | Especifica padrões de nível de classe respeitados por novas atribuições criadas na classe. |
|assignmentSettings| [coleção educationAssignmentSettings](educationassignmentsettings.md) | Especifica as configurações de atribuições de nível de classe. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationClass",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "String (identifier)",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```

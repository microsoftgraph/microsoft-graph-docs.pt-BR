---
title: Tipo de recurso educationClass
description: 'Representa uma aula em uma escola. O **recurso educationClass** corresponde ao grupo Microsoft 365 e compartilha a mesma ID. Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados. Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.  '
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3d1d6eb24e9d9b21ed8e828488ae306ec5c4bae549e51ecf0e69d63c5319e3a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54160055"
---
# <a name="educationclass-resource-type"></a>Tipo de recurso educationClass

Namespace: microsoft.graph

Representa uma aula em uma escola. O **recurso educationClass** corresponde ao grupo Microsoft 365 e compartilha a mesma ID. Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados. Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos

| Método                                                   | Tipo de retorno                                                 | Descrição                                                                                          |
| :------------------------------------------------------- | :---------------------------------------------------------- | :--------------------------------------------------------------------------------------------------- |
| [Listar educationClasses](../api/educationclass-list.md)   | Coleção [educationClass](../resources/educationclass.md) | Obter uma lista dos [objetos educationClass](../resources/educationclass.md) e suas propriedades.     |
| [Criar educationClass](../api/educationclass-post.md) | [educationClass](../resources/educationclass.md)            | Crie um novo [objeto educationClass.](../resources/educationclass.md)                                |
| [Obter educationClass](../api/educationclass-get.md)       | [educationClass](../resources/educationclass.md)            | Leia as propriedades e as relações de um [objeto educationClass.](../resources/educationclass.md) |
| [Atualizar educationClass](../api/educationclass-update.md) | [educationClass](../resources/educationclass.md)            | Atualize as propriedades de um [objeto educationClass.](../resources/educationclass.md)                 |
| [Excluir educationClass](../api/educationclass-delete.md) | None                                                        | [Exclua um objeto educationClass.](../resources/educationclass.md)                                  |
| [delta](../api/educationclass-delta.md)                  | Coleção [educationClass](../resources/educationclass.md) | Obter alterações incrementais na coleção de recursos.                                                  |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                           | Descrição                                                        |
| :------------------- | :--------------------------------------------- | :----------------------------------------------------------------- |
| id                   | String                                         | Identificador de objeto. Herdado da [entidade](../resources/entity.md). |
| displayName          | String                                         | Nome da aula.                                                 |
| mailNickname         | String                                         | Nome de email para enviar email a todos os membros, se essa propriedade estiver habilitada.    |
| description          | Cadeia de caracteres                                         | Descrição da aula.                                          |
| createdBy            | [identitySet](../resources/identityset.md)     | Entidade que criou a aula                                       |
| classCode            | Cadeia de caracteres                                         | Código de aula usada pela escola para identificar a aula.               |
| externalName         | Cadeia de caracteres                                         | Nome da aula no sistema de sincronização.                           |
| externalId           | Cadeia de caracteres                                         | ID da aula no sistema de sincronização.                           |
| externalSource       | educationExternalSource                        | Como essa aula foi criada. Os valores possíveis são: `sis` e `manual`.  |
| externalSourceDetail | Cadeia de caracteres                                         | O nome da fonte externa de onde esses recursos foram gerados. |
| grade                | Cadeia de caracteres                                         | Nível de nota da classe.                                          |
| term                 | [educationTerm](../resources/educationterm.md) | Termos dessa aula.                                               |

## <a name="relationships"></a>Relações

| Relação | Tipo                                                          | Descrição                                               |
| :----------- | :------------------------------------------------------------ | :-------------------------------------------------------- |
| group        | [group](../resources/group.md)                                | O objeto Microsoft 365 grupo subjacente.                |
| members      | Coleção [educationUser](../resources/educationuser.md)     | Todos os usuários da aula. Anulável.                         |
| schools      | Coleção [educationSchool](../resources/educationschool.md) | Todas as escolas às quais essa aula está associada. Anulável. |
| teachers     | Coleção [educationUser](../resources/educationuser.md)     | Todos os professores da aula. Anulável.                      |

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

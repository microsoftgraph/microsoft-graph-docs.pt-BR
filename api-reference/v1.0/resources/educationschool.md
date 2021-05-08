---
title: Tipo de recurso educationSchool
description: 'Recurso usado para gerenciar aulas, professores e alunos da escola representada.  '
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b076b38e52bb8a7eb93a9eef35c866fc58e0e29a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231854"
---
# <a name="educationschool-resource-type"></a>Tipo de recurso educationSchool

Namespace: microsoft.graph

Recurso usado para gerenciar aulas, professores e alunos da escola representada.

Herda de [educationOrganization](../resources/educationorganization.md).

## <a name="methods"></a>Métodos

| Método                                                     | Tipo de retorno                                                   | Descrição                                                                                            |
| :--------------------------------------------------------- | :------------------------------------------------------------ | :----------------------------------------------------------------------------------------------------- |
| [Listar educationSchools](../api/educationschool-list.md)    | Coleção [educationSchool](../resources/educationschool.md) | Obter uma lista dos [objetos educationSchool](../resources/educationschool.md) e suas propriedades.     |
| [Criar educationSchool](../api/educationschool-post.md) | [educationSchool](../resources/educationschool.md)            | Crie um novo [objeto educationSchool.](../resources/educationschool.md)                                |
| [Obter educationSchool](../api/educationschool-get.md)       | [educationSchool](../resources/educationschool.md)            | Leia as propriedades e as relações de um [objeto educationSchool.](../resources/educationschool.md) |
| [Atualizar educationSchool](../api/educationschool-update.md) | [educationSchool](../resources/educationschool.md)            | Atualize as propriedades de um [objeto educationSchool.](../resources/educationschool.md)                 |
| [Excluir educationSchool](../api/educationschool-delete.md) | Nenhum                                                          | Exclua um objeto [educationSchool](../resources/educationschool.md).                                  |
| [delta](../api/educationschool-delta.md)                   | Coleção [educationSchool](../resources/educationschool.md) | Obter alterações incrementais na coleção de recursos.                                                    |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                               | Descrição                                                                                                                                                          |
| :------------------- | :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| address              | [physicalAddress](../resources/physicaladdress.md) | Endereço da escola.                                                                                                                                               |
| createdBy            | [identitySet](../resources/identityset.md)         | Entidade que criou a escola.                                                                                                                                       |
| descrição          | String                                             | Descrição da escola. Herdado de [educationOrganization](../resources/educationorganization.md).                                                             |
| displayName          | String                                             | Nome de exibição da escola. Herdado de [educationOrganization](../resources/educationorganization.md).                                                            |
| externalId           | Cadeia de caracteres                                             | ID da escola no sistema de sincronização.                                                                                                                                      |
| externalPrincipalId  | Cadeia de caracteres                                             | ID da entidade de segurança no sistema de sincronização.                                                                                                                                   |
| externalSource       | educationExternalSource                            | Fonte de onde essa organização foi criada. Herdado de [educationOrganization](../resources/educationorganization.md). Os valores possíveis são: `sis` e `manual`. |
| externalSourceDetail | String                                             | O nome da fonte externa de onde esses recursos foram gerados.                                                                                                   |
| highestGrade         | Cadeia de caracteres                                             | Ensino de nível mais alto.                                                                                                                                                |
| id                   | String                                             | Identificador de objeto. Herdado da [entidade](../resources/entity.md).                                                                                                   |
| lowestGrade          | Cadeia de caracteres                                             | Ensino de nível mais baixo.                                                                                                                                                 |
| phone                | Cadeia de caracteres                                             | Número de telefone da escola.                                                                                                                                              |
| principalEmail       | Cadeia de caracteres                                             | Endereço de email da entidade de segurança.                                                                                                                                      |
| principalName        | Cadeia de caracteres                                             | Nome da entidade de segurança.                                                                                                                                               |
| schoolNumber         | Cadeia de caracteres                                             | Número da escola.                                                                                                                                                       |

## <a name="relationships"></a>Relações

| Relação       | Tipo                                                        | Descrição                                       |
| :----------------- | :---------------------------------------------------------- | :------------------------------------------------ |
| administrativeUnit | [administrativeUnit](../resources/administrativeunit.md)    | A administrativeUnit subjacente para essa escola. |
| classes            | Coleção [educationClass](../resources/educationclass.md) | Aulas ministradas na escola. Anulável.           |
| users              | Coleção [educationUser](../resources/educationuser.md)   | Usuários na escola. Anulável.                    |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationSchool",
  "baseType": "microsoft.graph.educationOrganization",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationSchool",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "lowestGrade": "String",
  "highestGrade": "String",
  "schoolNumber": "String",
  "externalId": "String",
  "phone": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```

---
title: Tipo de recurso educationSchool
description: 'Recurso usado para gerenciar aulas, professores e alunos da escola representada.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 407f29c7d8f9468c5e9b1da1badad294cb655121
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531513"
---
# <a name="educationschool-resource-type"></a>Tipo de recurso educationSchool

Namespace: microsoft.graph

Recurso usado para gerenciar aulas, professores e alunos da escola representada.  

## <a name="methods"></a>Métodos

| Método                                                   | Tipo de retorno                                    | Descrição                                                                                 |
| :------------------------------------------------------- | :--------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [Get](../api/educationschool-get.md)                     | [educationSchool](educationschool.md)          | Leia as propriedades e relações de um objeto **educationSchool**.                         |
| [Adicionar classe](../api/educationschool-post-classes.md)      | [educationClass](educationclass.md)            | Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.  |
| [Listar classes](../api/educationschool-list-classes.md)   | Coleção [educationClass](educationclass.md) | Obtenha a coleção de objetos **educationClass**.                                               |
| [Remover classe](../api/educationschool-delete-classes.md) | [educationClass](educationclass.md)            | Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.       |
| [Adicionar usuário](../api/educationschool-post-users.md)         | [educationUser](educationuser.md)              | Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**. |
| [Listar usuários](../api/educationschool-list-users.md)       | Coleção [educationUser](educationuser.md)   | Obtenha a coleção de objetos **educationUser**.                                                |
| [Remover usuário](../api/educationschool-delete-users.md)    | [educationUser](educationuser.md)              | Remova um **educationUser** da escola por meio da propriedade de navegação **users**.      |
| [Atualizar](../api/educationschool-update.md)               | [educationSchool](educationschool.md)          | Atualize um objeto **educationSchool**.                                                       |
| [Excluir](../api/educationschool-delete.md)               | Nenhum                                           | Exclua um objeto **educationSchool**.                                                       |

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                                  | Descrição                                                                        |
| :------------------ | :------------------------------------ | :--------------------------------------------------------------------------------- |
| id                  | String                                | GUID desta escola.                                                               |
| displayName         | Cadeia de caracteres                                | Nome de exibição da escola.                                                        |
| description         | String                                | Descrição da escola.                                                         |
| status              | cadeia de caracteres                                | Somente Leitura. Os valores possíveis são: `inactive`, `active`, `expired`, `deleteable`. |
| externalSource      | educationExternalSource               | Somente Leitura.  Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.        |
| principalEmail      | String                                | Endereço de email da entidade de segurança.                                                    |
| principalName       | String                                | Nome da entidade de segurança.                                                             |
| externalPrincipalId | String                                | ID da entidade de segurança no sistema de sincronização.                                                 |
| highestGrade        | String                                | Ensino de nível mais alto.                                                              |
| lowestGrade         | String                                | Ensino de nível mais baixo.                                                               |
| schoolNumber        | String                                | Número da escola.                                                                     |
| externalId          | Cadeia de caracteres                                | ID da escola no sistema de sincronização.                                                    |
| phone               | String                                | Número de telefone da escola.                                                            |
| address             | [physicalAddress](physicaladdress.md) | Endereço da escola.                                                             |
| createdBy           | [identitySet](identityset.md)         | Entidade que criou a escola.                                                     |

## <a name="relationships"></a>Relacionamento

| Relação | Tipo                                           | Descrição                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| classes      | Coleção [educationClass](educationclass.md) | Aulas ministradas na escola. Anulável. |
| users        | Coleção [educationUser](educationuser.md)   | Usuários na escola. Anulável.          |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.educationOrganization",
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

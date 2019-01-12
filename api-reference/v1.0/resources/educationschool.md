---
title: Tipo de recurso educationSchool
description: 'Recurso usado para gerenciar aulas, professores e alunos da escola representada.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 2549d8babd000a36f0ff3ccd38541ef3c1b2e466
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925816"
---
# <a name="educationschool-resource-type"></a>Tipo de recurso educationSchool

Recurso usado para gerenciar aulas, professores e alunos da escola representada.  


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter](../api/educationschool-get.md) | [educationSchool](educationschool.md) |Leia as propriedades e relações de um objeto **educationSchool**.|
|[Adicionar classe](../api/educationschool-post-classes.md) |[educationClass](educationclass.md)| Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.|
|[Listar classes](../api/educationschool-list-classes.md) |Coleção [educationClass](educationclass.md)| Obtenha a coleção de objetos **educationClass**.|
|[Remover classe](../api/educationschool-delete-classes.md) |[educationClass](educationclass.md)| Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.|
|[Adicionar usuário](../api/educationschool-post-users.md) |[educationUser](educationuser.md)| Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.|
|[Listar usuários](../api/educationschool-list-users.md) |Coleção [educationUser](educationuser.md)| Obtenha a coleção de objetos **educationUser**.|
|[Remover usuário](../api/educationschool-delete-users.md) |[educationUser](educationuser.md)| Remova um **educationUser** da escola por meio da propriedade de navegação **users**.|
|[Atualizar](../api/educationschool-update.md) | [educationSchool](educationschool.md) |Atualize um objeto **educationSchool**. |
|[Excluir](../api/educationschool-delete.md) | Nenhum |Exclua um objeto **educationSchool**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|GUID desta escola.|
|displayName| Cadeia de caracteres| Nome de exibição da escola.| 
|description| Cadeia de caracteres | Descrição da escola.| 
|status| string| Somente Leitura. Os valores possíveis são: `inactive`, `active`, `expired`, `deleteable`.|
|externalSource| educationExternalSource| Somente Leitura.  Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.|
|principalEmail| Cadeia de caracteres| Endereço de email da entidade de segurança.|
|principalName| Cadeia de caracteres | Nome da entidade de segurança.|
|externalPrincipalId| Cadeia de caracteres | ID da entidade de segurança no sistema de sincronização. |
|highestGrade|Cadeia de caracteres| Ensino de nível mais alto. |
|lowestGrade|Cadeia de caracteres| Ensino de nível mais baixo. |
|schoolNumber|Cadeia de caracteres| Número da escola.|
|externalId|Cadeia de caracteres| ID da escola no sistema de sincronização. |
|phone|Cadeia de caracteres| Número de telefone da escola. |
|fax|Cadeia de caracteres| Número de fax da escola. |
|address|[physicalAddress](physicaladdress.md)| Endereço da escola.|
|createdBy|[identitySet](identityset.md)|Entidade que criou a escola.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|classes|Coleção [educationClass](educationclass.md)| Aulas ministradas na escola. Anulável.|
|users|Coleção [educationUser](educationuser.md)| Usuários na escola. Anulável.|

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
  "fax": "String",
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

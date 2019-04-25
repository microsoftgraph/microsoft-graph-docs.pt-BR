---
title: Tipo de recurso educationSchool
description: 'Uma escola. O recurso **educationSchool** atualmente corresponde a um recurso administrativeUnit e compartilha a mesma ID.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 917395324e6ae519af468a4bb4b31056796e1498
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542911"
---
# <a name="educationschool-resource-type"></a>Tipo de recurso educationSchool

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma escola. O recurso **educationSchool** atualmente corresponde a um recurso [administrativeUnit](administrativeunit.md) e compartilha a mesma ID.  

Esse recurso é um subtipo de [educationOrganization](educationorganization.md).




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
|[Obter administrativeUnit](../api/educationschool-get-administrativeunit.md) |[administrativeUnit](administrativeunit.md)| Obtenha o **administrativeUnit** que corresponde a esse **educationSchool**.|
|[Atualizar](../api/educationschool-update.md) | [educationSchool](educationschool.md) |Atualize um objeto **educationSchool**. |
|[Excluir](../api/educationschool-delete.md) | Nenhum |Exclua um objeto **educationSchool**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|GUID desta escola.|
|displayName| String| Nome de exibição da escola.| 
|description| String | Descrição da escola.| 
|status| cadeia de caracteres| Somente Leitura. Os valores possíveis são: `inactive`, `active`, `expired`, `deleteable`.|
|externalSource| cadeia de caracteres| Somente Leitura.  Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.|
|principalEmail| String| Endereço de email da entidade de segurança.|
|principalName| String | Nome da entidade de segurança.|
|externalPrincipalId| String | ID da entidade de segurança no sistema de sincronização. |
|highestGrade|String| Ensino de nível mais alto. |
|lowestGrade|String| Ensino de nível mais baixo. |
|schoolNumber|String| Número da escola.|
|externalId|Cadeia de caracteres| ID da escola no sistema de sincronização. |
|phone|String| Número de telefone da escola. |
|fax|String| Número de fax da escola. |
|address|[physicalAddress](physicaladdress.md)| Endereço da escola.|
|createdBy|[identitySet](identityset.md)|Entidade que criou a escola.|


## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|classes|Coleção [educationClass](educationclass.md)| Aulas ministradas na escola. Anulável.|
|users|Coleção [educationUser](educationuser.md)| Usuários na escola. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationschool.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

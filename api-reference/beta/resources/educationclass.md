---
title: Tipo de recurso educationClass
description: 'Representa uma aula em uma escola. O recurso **educationClass** corresponde ao grupo do Office 365 e compartilha a mesma ID. Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados. Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f651e695ddf0b7139a31d077dcf021fced91293a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962916"
---
# <a name="educationclass-resource-type"></a>Tipo de recurso educationClass

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa uma aula em uma escola. O recurso **educationClass** corresponde ao grupo do Office 365 e compartilha a mesma ID. Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados. Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.  


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter educationClass](../api/educationclass-get.md) | [educationClass](educationclass.md) |Leia as propriedades e relações de um objeto **educationClass**.|
|[Adicionar membro](../api/educationclass-post-members.md) |[educationUser](educationuser.md)| Adicione um novo **educationUser** para a aula postando na propriedade de navegação de membros.|
|[Listar membros](../api/educationclass-list-members.md) |Coleção [educationUser](educationuser.md)| Obtenha uma coleção de objetos **educationUser**.|
|[Remover alunos](../api/educationclass-delete-members.md) |[educationUser](educationuser.md)| Remova um **educationUser** da aula por meio da propriedade de navegação de membros.|
|[Listar escolas](../api/educationclass-list-schools.md) |Coleção [educationSchool](educationschool.md)| Obtenha uma coleção de objetos **educationSchool**.|
|[Adicionar professor](../api/educationclass-post-teachers.md) |[educationUser](educationuser.md)| Adicione um novo **educationUser** para a aula postando na propriedade de navegação de professores.|
|[Listar professores](../api/educationclass-list-teachers.md) |Coleção [educationUser](educationuser.md)| Obtenha uma lista de professores para a aula.|
|[Remover professor](../api/educationclass-delete-teachers.md) |[educationUser](educationuser.md)| Remova um **educationUser** da aula por meio da propriedade de navegação de professores.|
|[Criar educationAssignment](../api/educationclass-post-assignments.md) |[educationAssignment](../resources/educationassignment.md)| Crie um novo **educationAssignment** pelo lançamento para a coleção assignments.|
|[Lista de atribuições](../api/educationclass-list-assignments.md) |coleção [educationAssignment](../resources/educationassignment.md)| Obtenha uma coleção de objetos **educationAssignment** .|
|[Obter grupo](../api/educationclass-get-group.md) |[group](group.md)| Recupere o **group** do Office 365 que corresponde a essa **educationClass**.|
|[Atualizar](../api/educationclass-update.md) | [educationClass](educationclass.md)    |Atualize o objeto **educationClass**. |
|[Excluir](../api/educationclass-delete.md) | Nenhum |Exclua o objeto **educationClass**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id| Cadeia de caracteres| O identificador exclusivo da aula.|
|description|Cadeia de caracteres| Descrição da aula.|
|displayName|Cadeia de caracteres| Nome da aula.|
|mailNickname|Cadeia de caracteres| Nome de email para enviar email a todos os membros, se essa propriedade estiver habilitada. |
|createdBy|[identitySet](identityset.md)| Entidade que criou a aula |
|classCode|Cadeia de caracteres| Código de aula usada pela escola para identificar a aula.|
|externalId|Cadeia de caracteres| ID da aula no sistema de sincronização. |
|externalName|Cadeia de caracteres|Nome da aula no sistema de sincronização.|
|externalSource|string| Como essa aula foi criada. Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.|
|term|[educationTerm](educationterm.md)|Termos dessa aula.|


## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|members|Coleção [educationUser](../resources/educationuser.md)| Todos os usuários da aula. Anulável.|
|schools|Coleção [educationSchool](../resources/educationschool.md)| Todas as escolas às quais essa aula está associada. Anulável.|
|teachers|Coleção [educationUser](../resources/educationuser.md)|  Todos os professores da aula. Anulável.|
|assignments|coleção [educationAssignment](../resources/educationassignment.md)| Todas as atribuições associadas a esta classe. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.education.term"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

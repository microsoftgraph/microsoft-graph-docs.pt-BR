---
title: Tipo de recurso educationRoot
description: 'O namespace `/education` expõe funcionalidade específica ao setor de educação. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 91f0162402b8c87042fab622710d314f27d6f4e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507144"
---
# <a name="educationroot-resource-type"></a>Tipo de recurso educationRoot

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O namespace `/education` expõe funcionalidade específica ao setor de educação. Alguns objetos no namespace `/education` podem ser encontrados em outras partes do Microsoft Graph (por exemplo, [usuários](user.md)). O namespace education fornece propriedades e recursos específicos de educação nesses objetos.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar educationClass](../api/educationroot-post-classes.md) |[educationClass](educationclass.md)| Crie uma nova **educationClass** postando na coleção de aulas.|
|[Listar classes](../api/educationroot-list-classes.md) |Coleção [educationClass](educationclass.md)| Obtenha uma coleção de objetos **educationClass**.|
|[Criar educationSchool](../api/educationroot-post-schools.md) |[educationSchool](educationschool.md)| Crie uma nova **educationSchool** postando na coleção de escolas.|
|[Listar escolas](../api/educationroot-list-schools.md) |Coleção [educationSchool](educationschool.md)| Obtenha uma coleção de objetos **educationSchool**.|
|[Criar educationUser](../api/educationroot-post-users.md) |[educationUser](educationuser.md)| Crie um novo **educationUser** postando na coleção de usuários.|
|[Listar usuários](../api/educationroot-list-users.md) |Coleção [educationUser](educationuser.md)| Obtenha uma coleção de objetos **educationUser**.|

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|classes|Coleção [educationClass](educationclass.md)| Somente leitura. Anulável.|
|me|[educationUser](educationuser.md)| Somente leitura. Anulável.|
|schools|Coleção [educationSchool](educationschool.md)| Somente leitura. Anulável.|
|users|Coleção [educationUser](educationuser.md)| Somente leitura. Anulável.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationroot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

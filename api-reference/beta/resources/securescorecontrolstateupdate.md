---
title: " tipo de recurso de secureScoreControlStateUpdate"
description: Este recurso contém o histórico de estados de controle atualizado por usuário (incluem de estados de controle padrão, Ignored, ThirdParty, revisado).
localization_priority: Normal
ms.openlocfilehash: 4e626f67579e3dc35fe36f5dcc67b1512c5e7bbc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574387"
---
 ##  <a name="securescorecontrolstateupdate-resource-type"></a>tipo de recurso de secureScoreControlStateUpdate

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Contém o histórico dos Estados controle atualizados pelo usuário (incluem de estados de controle padrão, Ignored, ThirdParty, revisado).

|Propriedade         | Tipo           |Descrição                                                  |
|:----------------|:---------------|:------------------------------------------------------------|
| assignedTo      | string         | Atribua o controle ao usuário que executará a ação     |
| comment         | string         | Fornece um comentário opcional sobre o controle                 |
| estado           | string         | Estado do controle pode ser modificado usando-se o comando de PATCH (ex.: ignorados, thirdParty etc.) |
| updatedBy       | string         |ID do usuário que atualizou o estado de locatário                      |
| updatedDateTime | DateTimeOffset |Tempo no qual controle estado foi atualizado                      |
 

## <a name="json-representation"></a>Representação JSON
 Veja a seguir uma representação JSON do recurso.

 <!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
```json
{
  "assignedTo": "String",
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
  "updatedDateTime": "DateTimeOffset"
}
```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

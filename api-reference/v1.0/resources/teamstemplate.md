---
title: Tipo de recurso teamsTemplate
description: Descreve a entidade teamsTemplate.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5adcd554c687747fb45cdfd1a40e9e37cfaad2d9107a43ebc2ceca01b5d94f3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249122"
---
# <a name="teamstemplate-resource-type"></a>Tipo de recurso teamsTemplate

Namespace: microsoft.graph

Um modelo de equipe é um modelo para criar uma [equipe](../resources/team.md) no Microsoft Teams. Um modelo especifica a estrutura, as configurações e até o conteúdo que deve ser provisionado em uma nova equipe criada usando o modelo. A Microsoft fornece um pacote de modelos básicos e os clientes podem salvar seus próprios modelos personalizados.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | Cadeia de caracteres   | Identificador exclusivo do modelo. Não pode ser nulo. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

## <a name="see-also"></a>Confira também

- [equipe](team.md)



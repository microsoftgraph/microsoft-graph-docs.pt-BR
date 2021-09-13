---
title: Tipo de recurso teamsTemplate
description: Descreve a entidade teamsTemplate.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3ef812716b2650e7919d18291f1f43c9adf878b5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098409"
---
# <a name="teamstemplate-resource-type"></a>Tipo de recurso teamsTemplate

Namespace: microsoft.graph

Um modelo de equipe é um modelo para criar uma [equipe](../resources/team.md) no Microsoft Teams. Um modelo especifica a estrutura, as configurações e até o conteúdo que deve ser provisionado em uma nova equipe criada usando o modelo. A Microsoft fornece um pacote de modelos básicos e os clientes podem salvar seus próprios modelos personalizados.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | String   | Identificador exclusivo do modelo. Não pode ser nulo. |

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



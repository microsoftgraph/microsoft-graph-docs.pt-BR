---
title: tipo de recurso de teamsTemplate
description: Descreve a entidade teamsTemplate.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 6e847c7ef0b13dd9c4281c17939164128be8b6a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818869"
---
# <a name="teamstemplate-resource-type"></a>tipo de recurso de teamsTemplate

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Um modelo de equipe é um blueprint para a criação de uma [equipe](../resources/team.md) no Microsoft Teams. Um modelo especifica a estrutura, configurações e até mesmo conteúdo que deve ser provisionado em uma nova criada usando o modelo de equipe. A Microsoft fornece um pacote de modelos de base e os clientes podem salvar seus próprios modelos personalizados.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | Cadeia de caracteres   | Identificador exclusivo do modelo. Não pode ser nula. |

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

# <a name="see-also"></a>Confira também

- [equipe](team.md)


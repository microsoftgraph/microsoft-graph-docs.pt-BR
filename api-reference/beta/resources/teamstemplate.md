---
title: tipo de recurso de teamsTemplate
description: Descreve a entidade teamsTemplate.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9bd5047950ed1ed3c57950d2c4b708a78b570649
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940082"
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


---
title: tipo de recurso de ideias de pesquisas
description: Ideias são relações calculadas usando análises avançadas e técnicas de aprendizagem da máquina. Você pode, por exemplo, identificar documentos OneDrive tendências em torno de usuários.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 38f7afb40c1618a8a7cf9d585c99633e2bb8d940
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938311"
---
# <a name="insights-resource-type"></a>tipo de recurso de ideias de pesquisas

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Ideias são relações calculadas usando análises avançadas e técnicas de aprendizagem da máquina. Você pode, por exemplo, identificar documentos OneDrive tendências em torno de usuários.

Ideias são retornadas pelas seguintes APIs:

- [Tendência](insights-trending.md) - retornará documentos do OneDrive e de sites do SharePoint tendências em torno de um usuário.
- [Usado](insights-used.md) - retornará documentos exibidos e modificados por um usuário. Inclui os documentos que o usuário tiver usado no OneDrive for Business, SharePoint, abertos como anexos de email e como anexos de link de fontes como caixa, pasta de recados e Google unidade.
- [Shared](insights-shared.md) - retorna documentos compartilhados com um usuário. Documentos podem ser compartilhados como anexos de email ou OneDrive for Business vincula emails enviados no.

Cada insight é retornado com um `resourceVisualization` e `resourceReference` o tipo de valor complexa (CVT). O resourceVisualization CVT contém propriedades tais como `title` e `previewImageUrl`. A Microsoft usa as propriedades de visualização para processar os arquivos em experiências como Office me aprofundar.

## <a name="relationships"></a>Relações

| Relação      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| análise de tendências      | Coleção de [tendência](insights-trending.md)       | Relacionamento calculado identificar tendências de documentos. Tendências de documentos podem ser armazenados em OneDrive ou em sites do SharePoint.   |
| used      | Coleção [usado](insights-used.md)       | Calculado relação identificar documentos exibidos e modificados por um usuário. Inclui os documentos que o usuário tiver usado no OneDrive for Business, SharePoint, abertos como anexos de email e como anexos de link de fontes como caixa, pasta de recados e Google unidade.  |
| shared        | Coleção [compartilhados](insights-shared.md)       | Relacionamento calculado identificando documentos compartilhados com um usuário. Documentos podem ser compartilhados como anexos de email ou OneDrive for Business vincula emails enviados no.   |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso
```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```

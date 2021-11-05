---
title: tipo de recurso itemInsights
description: Relacionamentos entre um usuário e itens como documentos do OneDrive for Business, calculados usando análises avançadas e técnicas de aprendizado de máquina. Por exemplo, você pode identificar tendências de documentos do OneDrive for Business entre usuários à sua volta.
author: simonhult
ms.localizationpriority: high
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 74452522b77e240c398c80a4dc8bec9c377efb09
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780923"
---
# <a name="iteminsights-resource-type"></a>tipo de recurso itemInsights

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Relacionamentos entre um usuário e itens como documentos do OneDrive for Business, calculados usando análises avançadas e técnicas de aprendizado de máquina. Por exemplo, você pode identificar tendências de documentos do OneDrive for Business entre usuários à sua volta. Derivados do [officeGraphInsights](officegraphinsights.md).

Informações são retornadas pelas seguintes APIs:

- [Tendências](insights-trending.md) - retorna documentos do OneDrive for Business e de sites do SharePoint tendendo para um usuário.
- [Usadas](insights-used.md) - retorna documentos exibidos e modificados recentemente por um usuário. Inclui documentos que o usuário usou no OneDrive for Business e no SharePoint.
- [Compartilhado](insights-shared.md) -retornará documentos compartilhados com um usuário. Documentos podem ser compartilhados como anexos de email ou links do OneDrive para Business enviados por email.

Cada ideia é retornada com um tipo de valor complexo (CVT) `resourceVisualization` e `resourceReference`. O resourceVisualization CVT contém propriedades, como `title` e `previewImageUrl`. A Microsoft usa as propriedades de visualização para renderizar os arquivos em experiências como o Office Delve.

### <a name="limiting-item-insights"></a>Limitando as informações do item

Atualize [insightsSettings](insightssettings.md) para desabilitar insights de item para um grupo específico do Microsoft Azure AD ou de uma organização inteira. Para obter mais detalhes, confira [personalizar política de informações](/graph/insights-customize-item-insights-privacy).

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

| Relação      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| tendências      | coleção [tendências](insights-trending.md)        | Relacionamento calculado que identifica documentos de tendências em torno de um usuário. Os documentos de tendência são calculados com base na atividade da rede de pessoas mais próximas do usuário e incluem arquivos armazenados no OneDrive for Business e no SharePoint. As informações de tendências ajudam o usuário a descobrir o conteúdo potencialmente útil que ele tem acesso, mas nunca viu antes.|
| usado      | coleção [usedInsight](insights-used.md)        | Relacionamento calculado que identifica os documentos mais recentes exibidos e modificados por um usuário, incluindo documentos do OneDrive for Business e do SharePoint, classificados por tempo de uso recente.|
| compartilhado        | coleção [sharedInsight](insights-shared.md)        | Relação calculada que identifica documentos compartilhados com ou pelo usuário, inclui anexos de arquivo em emails e reuniões, bem como URLs e anexos de referência para OneDrive for Business e arquivos do Microsoft Office SharePoint Online encontrados em emails, reuniões e conversas de equipes. Ordenado por tempo para retorno do compartilhamento.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso
<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "baseType":"microsoft.graph.officeGraphInsights",
  "optionalProperties": [
    "trending",
    "used",
    "shared"
  ],
  "@odata.type": "microsoft.graph.itemInsights"
}-->

```json
{
  "id": "string",
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```



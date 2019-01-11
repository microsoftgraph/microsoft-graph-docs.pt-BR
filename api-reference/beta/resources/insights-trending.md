---
title: tipo de recurso de tendências
description: Relacionamento de rich conectando a um usuário a documentos que são tendências em torno do usuário (são relevante para o usuário). Arquivos de OneDrive, os arquivos armazenados em sites de equipe do SharePoint podem tendências em torno do usuário e.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: dc0154d3985e5f6e1e4770bb7d10bc727a0eb0ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862381"
---
# <a name="trending-resource-type"></a>tipo de recurso de tendências

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Relacionamento de rich conectando a um usuário a documentos que são tendências em torno do usuário (são relevante para o usuário). Arquivos de OneDrive, os arquivos armazenados em sites de equipe do SharePoint podem tendências em torno do usuário e.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Lista de tendências](../api/insights-list-trending.md) |coleção [insights_trending](insights-trending.md)| Obtenha uma lista dos arquivos de tendências.|

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                              | Descrição  |
| ------------- |---------------                    | -------------|
| id                    | Cadeia de caracteres                    | Identificador exclusivo do relacionamento. Somente leitura.        |
| weight                | Duplo                    | Valor que indica o quanto o documento está atualmente tendências. Quanto maior o número, mais o documento é atualmente tendências ao redor do usuário (o mais relevantes é). Documentos retornados são classificados por esse valor.  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)    | Propriedades que você pode usar para visualizar o documento na sua experiência. |
| resourceReference     | [resourceReference](insights-resourcereference.md)        | Propriedades de referência do documento tendência, como a url e o tipo de documento. |

## <a name="relationships"></a>Relações

| Propriedade      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| recurso      | Entity        | Usado para navegar até o documento tendência. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```

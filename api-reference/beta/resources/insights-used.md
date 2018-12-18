---
title: usado o tipo de recurso
description: Uma compreensão dos representando documentos usados por um usuário específico. As ideias retorna os documentos mais relevantes que um usuário visualizados ou acessados.
author: simonhult
ms.openlocfilehash: 89eac33ad954905c77a26df669bb15a2cf471edd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323482"
---
# <a name="used-resource-type"></a>usado o tipo de recurso

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Uma compreensão dos representando documentos usados por um usuário específico. As ideias retorna os documentos mais relevantes que um usuário visualizados ou acessados. Isso inclui documentos em:

- OneDrive for Business
- SharePoint

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Lista usada](../api/insights-list-used.md) |coleção [insights_used](insights-used.md)| Obtenha uma lista de arquivos utilizados.|

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                      | Descrição  |
| -------------         |---------------            | -------------|
| id                    | String                    | Identificador exclusivo do relacionamento. Somente leitura.        |
| lastUsed              | [usageDetails](insights-usagedetails.md)              | Informações sobre quando o item foi último exibidos e modificados pelo usuário. Somente leitura.     |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Propriedades que você pode usar para visualizar o documento na sua experiência. Somente leitura      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Propriedades de referência do documento usado, como a url e o tipo de documento. Somente leitura     |

## <a name="relationships"></a>Relações

| Propriedade      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| recurso      | Entity        | Usado para navegar até o item que foi usado. Anexos de arquivo, o tipo é *fileAttachment*. Anexos vinculados, o tipo é *driveItem*. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
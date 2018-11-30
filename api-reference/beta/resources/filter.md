---
title: Tipo de recurso Filter
description: Gerencia a filtragem da coluna de uma tabela.
ms.openlocfilehash: df896d10b1e8734015d38b92b5824e3e3652e3a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037734"
---
# <a name="filter-resource-type"></a>Tipo de recurso Filter

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Gerencia a filtragem da coluna de uma tabela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Aplicar](../api/filter-apply.md)|Nenhum|Aplica os critérios de filtro determinados à coluna fornecida.|
|[Clear](../api/filter-clear.md)|Nenhum|Limpa o filtro na coluna determinada.|

## <a name="properties"></a>Propriedades
Nenhum

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|critérios|[FilterCriteria](filtercriteria.md)|O filtro aplicado no momento à coluna fornecida. Somente leitura.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
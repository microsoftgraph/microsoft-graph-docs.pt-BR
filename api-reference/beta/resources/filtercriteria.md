---
title: Tipo de recurso FilterCriteria
description: Representa os critérios de filtragem aplicados a uma coluna.
ms.openlocfilehash: dbcc57ff940fec525b712eb11ac44209f5f8a4d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033836"
---
# <a name="filtercriteria-resource-type"></a>Tipo de recurso FilterCriteria

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa os critérios de filtragem aplicados a uma coluna.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterCriteria"
}-->

```json
{
  "color": "string",
  "criterion1": "string",
  "criterion2": "string",
  "dynamicCriteria": "string",
  "filterOn": "string",
  "values": "string"
}

```
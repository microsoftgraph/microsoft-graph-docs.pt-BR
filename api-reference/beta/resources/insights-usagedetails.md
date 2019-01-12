---
title: tipo de recurso usageDetails
description: Tipo complexo que contém as propriedades de itens usados. Obter informações sobre quando o recurso foi acessado pela última vez (exibidos) e modificado (editado) pelo usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 466308ad1b6290c2b96335f94c586eb35c6cac28
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950015"
---
# <a name="usagedetails-resource-type"></a>tipo de recurso usageDetails

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Tipo complexo que contém as propriedades de itens [usado](insights-used.md) . Obter informações sobre quando o recurso foi acessado pela última vez (exibidos) e modificado (editado) pelo usuário.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo          | Descrição  |
| -------------         |---------------| -------------|
| lastAccessedDateTime                  | DateTimeOffset        | A data e hora que o recurso foi acessado pela última vez pelo usuário. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`. Somente leitura.                      |
| lastModifiedDateTime              | DateTimeOffset        | A data e hora que o recurso da última modificação pelo usuário. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`. Somente leitura.       |

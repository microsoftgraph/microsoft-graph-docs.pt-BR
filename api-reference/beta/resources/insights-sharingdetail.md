---
title: tipo de recurso de sharingDetail
description: 'Tipo complexo que contém as propriedades de itens compartilhados. '
author: simonhult
ms.openlocfilehash: 8454fd451f0659ff3ccad270df3414a850bee180
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353372"
---
# <a name="sharingdetail-resource-type"></a>tipo de recurso de sharingDetail

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Tipo complexo que contém as propriedades de itens [compartilhados](insights-shared.md) . 

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso

```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo          | Descrição  |
| -------------         |-----------    | -------------|
| sharedDateTime        | DateTimeOffset| A data e hora que o arquivo foi última compartilhado. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`. Somente leitura.  |
| sharingSubject        | String          | O assunto com a qual o documento foi compartilhado. |
| sharingType             | String        | Determina a maneira como o documento foi compartilhada, pode ser um "Link", por "Anexo", "Grupo", "Site".     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | O usuário que compartilhado do documento.  |
| sharingReference        | [resourceReference](insights-resourcereference.md)      |  |
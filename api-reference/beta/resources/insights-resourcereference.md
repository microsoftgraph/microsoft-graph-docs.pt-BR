---
title: tipo de recurso de resourceReference
description: Tipo complexo que contém propriedades de ideias.
ms.openlocfilehash: d171151a1c3547aa6863a7f70cc3a42ddec13e5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037946"
---
# <a name="resourcereference-resource-type"></a>tipo de recurso de resourceReference

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Tipo complexo que contém propriedades de [ideias](insights.md).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição  |
| ------------- |-----------| -------------|
| webUrl        | String    | Uma URL, levando a item referenciado. |
| id            | String    | Identificador exclusivo do item.           |
| type          | String    | Um valor de cadeia de caracteres que pode ser usado para classificar o item, como "microsoft.graph.driveItem" |
---
title: insightIdentity
description: Tipo complexo que contém as propriedades de itens compartilhados.
author: simonhult
ms.openlocfilehash: 648242b827c0390029522955b0fe6347b98100c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331329"
---
# <a name="insightidentity"></a>insightIdentity

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Tipo complexo que contém as propriedades de itens [compartilhados](insights-shared.md) . 

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo          | Descrição  |
| -------------         |-----------    | -------------|
| displayName       | String          | O nome de exibição do usuário que shared o item. |
| id              | String        | A identificação do usuário que shared o item.     |
| address             | Cadeia de caracteres      | O endereço de email do usuário que shared o item.  |
---
title: insightIdentity
description: " tipo de recurso"
ms.openlocfilehash: e13d08eb111844896c96b02ab22c52d2f598ce58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037747"
---
# <a name="insightidentity"></a>insightIdentity

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

 tipo de recurso

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
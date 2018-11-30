---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Raiz
ms.openlocfilehash: 771eb39baf2a7ce7a85fb43120d6e9e7358f6f6c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036877"
---
# <a name="root-resource-type"></a>Tipo de recurso Root

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

A faceta **Root** indica que um objeto é o mais alto em sua hierarquia.
A presença (não nulo) do valor da faceta indica que o objeto é a raiz.
Um valor nulo (ou ausente) indica que o objeto não é a raiz.

**Observação**: Embora essa faceta esteja vazia no momento, em revisões futuras da API a faceta pode ser preenchida com propriedades adicionais.

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a>Propriedades

O recurso **Root** não tem propriedades.


<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/Root"
} -->

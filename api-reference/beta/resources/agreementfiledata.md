---
title: Tipo de recurso agreementFileData
description: Representa o blob de um arquivo de contrato de Azure Active Directory (Azure AD).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 3fa6c94497ae42b102f03bee6142ec38677eda93
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451309"
---
# <a name="agreementfiledata-resource-type"></a>Tipo de recurso agreementFileData

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o blob de um arquivo de contrato de Azure Active Directory (Azure AD).

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo | Descrição |
|:-------------|:------------|:------------|
|data|Binária|Dados que representam os termos de uso do documento PDF. Somente leitura. <br/><br/>**Observação:** Você pode usar o método .NET [Convert.ToBase64String](/dotnet/api/system.convert.tobase64string) para converter seu arquivo em dados binários para carregar usando a API [Criar contratos](../api/termsofusecontainer-post-agreements.md) . Uma sintaxe de exemplo que usa esse método no PowerShell é `[convert]::ToBase64String((Get-Content -path "your_file_path" -Encoding byte))`. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



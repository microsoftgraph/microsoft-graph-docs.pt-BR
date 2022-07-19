---
title: Tipo de recurso tenantAllowBlockListEntryResult
description: Representa um resultado de entrada de lista de bloqueios de permissão de locatário.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 9e5a92fbc215c814ce2f55a1e9a16407bc60f147
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856518"
---
# <a name="tenantallowblocklistentryresult-resource-type"></a>Tipo de recurso tenantAllowBlockListEntryResult

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o resultado de uma entrada de lista de bloqueios de permissão de locatário. Uma entrada para um item de lista de bloqueio de permissão de locatário pode ser uma URL, anexo ou remetentes.

## <a name="properties"></a>Propriedades
| Propriedade           | Tipo                          | Descrição                                             |
|:-------------------|:------------------------------|:--------------------------------------------------------|
| Entrytype          | tenantAllowBlockListEntryType | O tipo de entrada da lista de bloqueios de permissão de locatário. Os valores possíveis são: `url`, `fileHash`, `sender`e `unkownFutureValue``recipient` .  |
| expirationDateTime | DateTimeOffset                | Especifica quando essa entrada expirará na data e hora. |
| Identidade           | Cadeia de caracteres                        | Especifica a identidade da entrada gerada pelo sistema de lista de bloqueios de permissão do locatário. |
| status             | Longrunningoperationstatus    | Especifica se a operação de criação de entrada de lista de bloqueios de permissão de locatário foi bem-sucedida. Os valores possíveis são: `notStarted`, `running`, `succeeded`, `failed`e `unkownFutureValue``skipped` . |
| value              | Cadeia de caracteres                        | Especifica o valor da entrada da lista de bloqueios de permissão do locatário criado.  |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.tenantAllowBlockListEntryResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.tenantAllowBlockListEntryResult",
  "identity": "String",
  "value": "String",
  "entryType": "String",
  "expirationDateTime": "String (timestamp)",
  "status": "String"
}
```


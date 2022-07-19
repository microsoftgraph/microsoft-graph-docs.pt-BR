---
title: Tipo de recurso tenantAllowOrBlockListAction
description: Representa a ação permitir ou bloquear lista de locatários
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 26dc913078122a1bbb994369e63e2e2c0336f6c0
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856569"
---
# <a name="tenantalloworblocklistaction-resource-type"></a>Tipo de recurso tenantAllowOrBlockListAction

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a ação de lista de permissões ou bloqueios do locatário. Quando um administrador cria um envio de ameaças por email, uma operação de lista de bloqueios de permissão de locatário também pode ser fornecida. Quando uma operação de lista de bloqueios de permissão de locatário for fornecida, o envio de ameaças adicionará automaticamente itens relacionados (URLs, anexos, remetentes) à lista de bloqueios de permissão do locatário.

## <a name="properties"></a>Propriedades
| Propriedade           | Tipo                                        | Descrição                                                                      |
|:-------------------|:--------------------------------------------|:---------------------------------------------------------------------------------|
| ação             | tenantAllowBlockListAction                  | Especifica se a lista de bloqueios de permissão de locatário é um bloco ou permissão. Os valores possíveis são `allow`, `block` e `unkownFutureValue`.|
| expirationDateTime | DateTimeOffset                              | Especifica quando a lista de bloqueios permitidos do locatário expira na data e hora.  |
| Nota               | Cadeia de caracteres                                      | Especifica a anotação adicionada ao locatário permitir entrada de lista de blocos no formato de cadeia de caracteres. |
| Resultados            | Collection([security.tenantAllowBlockListEntryResult](../resources/security-tenantallowblocklistentryresult.md)) | Contém o resultado do envio que leva à criação da entrada de lista de bloqueios de locatário. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.tenantAllowOrBlockListAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.tenantAllowOrBlockListAction",
  "action": "String",
  "results": [
    {
      "@odata.type": "microsoft.graph.security.tenantAllowBlockListEntryResult"
    }
  ],
  "expirationDateTime": "String (timestamp)",
  "note": "String"
}
```


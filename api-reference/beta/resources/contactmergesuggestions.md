---
title: Tipo de recurso contactMergeSuggestions
description: Representa o recurso para sugerir a mesclação de itens de contato quando Outlook detecta duplicatas na lista de contatos do usuário
author: kevinbellinger
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 56237901cca14d075dfa7f03729a9261d8d281a0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338059"
---
# <a name="contactmergesuggestions-resource-type"></a>Tipo de recurso contactMergeSuggestions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o recurso para sugerir a mesclação de itens de contato quando Outlook detecta duplicatas na lista de contatos do usuário.

Esse recurso fornece um meio para habilitar ou desabilitar o recurso no nível do usuário. Por padrão, a sugestão está habilitada. Os itens de contato duplicados permanecem como duplicatas na pasta de contato, a menos que o usuário selecione mesclar eles.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Get](../api/contactmergesuggestions-get.md)|[contactMergeSuggestions](contactmergesuggestions.md)|Leia as propriedades de um **objeto contactMergeSuggestions** .|
|[Atualizar](../api/contactmergesuggestions-update.md)|Nenhum(a) |Atualize as propriedades de **um objeto contactMergeSuggestions** .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isEnabled|Booliano|`true` se o recurso de sugestões de mesclagem de contato duplicado estiver habilitado para o usuário; `false` se o recurso estiver desabilitado. O valor padrão é `true`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactMergeSuggestions",
  "openType": false
}
-->
``` json
{
  "isEnabled": "Boolean"
}
```


---
title: tipo de recurso educationFileSynchronizationVerificationMessage
description: Representa um erro retornado ao cliente em resposta a uma solicitação para iniciar a sincronização de perfis de dados escolares baseados em CSV. O recurso conterá erros resultantes da verificação. Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b65335538453f35457d5e83c49f7ba7c830d6a43
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095433"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>tipo de recurso educationFileSynchronizationVerificationMessage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um erro retornado ao cliente em resposta a uma solicitação para [iniciar a sincronização](../api/educationsynchronizationprofile-start.md) de perfis de dados escolares baseados em CSV. O recurso conterá erros resultantes da verificação. Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (Azure AD).

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo   | Descrição                                                                  |
| :---------- | :----- | :--------------------------------------------------------------------------- |
| type        | string | Tipo da mensagem. Os valores possíveis são: `error`, `warning`, `information`. |
| nomes    | cadeia de caracteres | Arquivo de origem que contém o erro.                                         |
| description | string | Informações detalhadas sobre o tipo de mensagem.                                 |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage"
}-->

```json
{
  "type": "String",
  "fileName": "String",
  "description": "String"
}
```



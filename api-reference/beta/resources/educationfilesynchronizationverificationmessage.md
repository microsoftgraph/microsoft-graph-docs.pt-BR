---
title: tipo de recurso de educationFileSynchronizationVerificationMessage
description: Representa um erro retornado ao cliente em resposta a uma solicitação para iniciar a sincronização de perfis de dados baseada em CSV escola. O recurso irá conter erros resultantes da verificação. Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (AD Azure).
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: ae09ec3f208adfee64a6392db9732841fc7a0808
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845511"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>tipo de recurso de educationFileSynchronizationVerificationMessage

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um erro retornado ao cliente em resposta a uma solicitação para [Iniciar a sincronização](../api/educationsynchronizationprofile-start.md) de perfis de dados baseada em CSV escola. O recurso irá conter erros resultantes da verificação. Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (AD Azure).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **type** | string | Tipo da mensagem. Os valores possíveis são: `error`, `warning`, `information`. | 
| **FileName** | string | Arquivo de origem que contém o erro. |
| **description** | string | Informações detalhadas sobre o tipo de mensagem. |

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

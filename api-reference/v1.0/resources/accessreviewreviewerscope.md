---
title: Tipo de recurso accessReviewReviewerScope
description: Representa quem revisará uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 55f881ff1bcb1b08cc66938fd8a7b4d28f540687
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469514"
---
# <a name="accessreviewreviewerscope-resource-type"></a>Tipo de recurso accessReviewReviewerScope

Namespace: microsoft.graph

O accessReviewReviewerScope define quem é especificado no [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) para revisar [appConsentRequests](../resources/appconsentrequest.md) e [userConsentRequests](../resources/appconsentrequest.md). Isso é expresso como uma consulta OData, que permite que os revisadores sejam especificados como uma lista estática de usuários (ou seja, usuários específicos, proprietários de grupo, membros do grupo) ou dinamicamente (ou seja, o caso em que cada usuário é revisado por seu gerente).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|consulta|String|A consulta especificando quem será o revistor. Consulte tabela para exemplos. |
|queryRoot|String|O tipo de consulta. Exemplos incluem `MicrosoftGraph` `ARM` e .|
|queryType|String|No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta. Essa propriedade só será necessária se uma consulta relativa (ou seja, `./manager` ) for especificada.|

### <a name="supported-queries-for-accessreviewreviewerscope"></a>Consultas com suporte para accessReviewReviewerScope

|Cenário| consulta | queryType | queryRoot |
|--|--|--|--|
| Proprietário do grupo como revistor | /groups/{group id}/owners |MicrosoftGraph||
| Usuário específico como revistor | /users/{user id} |MicrosoftGraph||
| Gerente do usuário que está sendo revisado como revistor | ./manager | MicrosoftGraph |decisions|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewReviewerScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewerScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```

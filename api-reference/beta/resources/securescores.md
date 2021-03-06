---
title: tipo de recurso secureScore
description: 'Top = n, onde n = o número de dias de dados que você deseja recuperar. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 3db31203f9c5827459ab2149efbd3adb28030d0a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087541"
---
# <a name="securescore-resource-type"></a>tipo de recurso secureScore

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível do locatário e do controle. Por padrão, são mantidos 90 dias de dados. Esses dados são classificados por **createdDateTime**, do mais recente para o mais antigo. Isso permitirá respostas de página usando $top = n, onde n = o número de dias de dados que você deseja recuperar.


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Listar secureScores](../api/securescores-list.md) | [secureScores](securescores.md) |Leia as propriedades e os metadados de um objeto secureScores.|


## <a name="properties"></a>Propriedades
Tipo de entidade contendo propriedades da Pontuação de segurança do locatário (dados de instantâneos diários).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|   azureTenantId   |   String  |   Cadeia de caracteres GUID para ID do locatário.  |
|   createdDateTime |   DateTimeOffset  |   A data em que a entidade é criada.  |
|   id  |   Cadeia de caracteres  |   Combinação de azureTenantId_createdDateTime.   |
|   licensedUserCount   |   Int32   |   Contagem de usuários licenciados de um determinado locatário.    |
|   activeUserCount |   Int32   |   Contagem de usuários ativos de um determinado locatário.  |
|   currentScore    |   Duplo  |   Pontuação Obtida de locatário atual em data especificada.    |
|   maxScore |  Duplo  |   Pontuação máxima possível de locatário na data especificada.    |
|   enabledservices |   Coleção String   |   Serviços fornecidos pela Microsoft para o locatário (por exemplo, Exchange Online, Skype, SharePoint).   |
|   averageComparativeScores |  coleção [averageComparativeScore](averagecomparativescore.md)    |Pontuação média por escopos diferentes (por exemplo, média por setor, média por meio de assentos) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura) dentro do escopo. |
|   controlScores | coleção [controlScore](controlscore.md)  |   Contém pontuações de locatários para um conjunto de controles.   |


## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
}-->

```json
{
  "id": "String",
  "azureTenantId": "Guid",
  "createdDate": "DateTimeOffset",
  "licensedUserCount": "Int32",
  "activeUserCount": "Int32",
  "currentScore": "Int32",
  "maxScore": "Int32",
  "averageScore": "Double",
  "enabledServices": "Collection(string)",
  "averageComparativeScores": "Collection(microsoft.graph.SecureScore.averageComparativeScores)",
  "controlScores": "Collection(microsoft.graph.SecureScore.controlScores)",
  "createdDateTime": "2019-02-07T20:33:53.156Z"
}

```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



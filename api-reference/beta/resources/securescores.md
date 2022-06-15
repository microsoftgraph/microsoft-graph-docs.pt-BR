---
title: Tipo de recurso secureScore
description: 'top=n, em que n = o número de dias de dados que você deseja recuperar. '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: 9565a507eac6d5c1be272749a45c6e4b234d5da2
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094092"
---
# <a name="securescore-resource-type"></a>Tipo de recurso secureScore

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível de locatário e controle. Por padrão, 90 dias de dados são mantidos. Esses dados são classificados por **createdDateTime**, do mais recente ao mais antigo. Isso permitirá que você page as respostas usando $top=n, em que n = o número de dias de dados que você deseja recuperar.


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Listar secureScores](../api/securescores-list.md) | [secureScores](securescores.md) |Ler propriedades e metadados de um objeto secureScores.|


## <a name="properties"></a>Propriedades
Tipo de entidade que contém propriedades da pontuação de segurança do locatário (dados de instantâneo diários).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|   activeUserCount |   Int32   |   Contagem de usuários ativos do locatário determinado.  |
|   averageComparativeScores |  [coleção averageComparativeScore](averagecomparativescore.md)    |Pontuação média por escopos diferentes (por exemplo, média por setor, média por assento) e categoria de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura) dentro do escopo. |
|   azureTenantId   |   String  |   Cadeia de caracteres GUID para a ID do locatário.  |
|   controlScores | [Coleção controlScore](controlscore.md)  |   Contém pontuações de locatário para um conjunto de controles.   |
|   createdDateTime |   DateTimeOffset  |   A data em que a entidade é criada.  |
|   currentScore    |   Duplo  |   Pontuação atual do locatário obtido na data especificada.    |
|   enabledServices |   Coleção String   |   Serviços fornecidos pela Microsoft para o locatário (por exemplo, Exchange online, Skype, SharePoint).   |
|   id  |   Cadeia de caracteres  |   Combinação de azureTenantId_createdDateTime.   |
|   licensedUserCount   |   Int32   |   Contagem de usuários licenciados do locatário especificado.    |
|   maxScore |  Duplo  |   Pontuação máxima possível do locatário na data especificada.    |




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
  "activeUserCount": "Int32",
  "averageComparativeScores": "Collection(microsoft.graph.SecureScore.averageComparativeScores)",
  "averageScore": "Double",
  "azureTenantId": "Guid",
  "controlScores": "Collection(microsoft.graph.SecureScore.controlScores)",
  "createdDate": "DateTimeOffset",
  "createdDateTime": "2019-02-07T20:33:53.156Z",
  "currentScore": "Int32",
  "enabledServices": "Collection(string)",
  "id": "String",
  "licensedUserCount": "Int32",
  "maxScore": "Int32"
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



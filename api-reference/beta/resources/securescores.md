---
title: Tipo de recurso secureScore
description: 'top=n, em que n = o número de dias de dados que você deseja recuperar. '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: f289ef7c91dbe7975970e679d1950a03498ab333
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900125"
---
# <a name="securescore-resource-type"></a>Tipo de recurso secureScore

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível de locatário e controle. Por padrão, 90 dias de dados são mantidos. Esses dados são classificados por **createdDateTime**, do mais recente ao mais antigo. Isso permitirá que você page as respostas usando $top=n, em que n = o número de dias de dados que você deseja recuperar.


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Lista secureScores](../api/securescores-list.md) | [secureScores](securescores.md) |Ler propriedades e metadados de um objeto secureScores.|


## <a name="properties"></a>Propriedades
Tipo de entidade que contém propriedades da pontuação de segurança do locatário (dados de instantâneo diários).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|   azureTenantId   |   String  |   Cadeia de caracteres GUID para a ID do locatário.  |
|   createdDateTime |   DateTimeOffset  |   A data em que a entidade é criada.  |
|   id  |   String  |   Combinação de azureTenantId_createdDateTime.   |
|   licensedUserCount   |   Int32   |   Contagem de usuários licenciados do locatário especificado.    |
|   activeUserCount |   Int32   |   Contagem de usuários ativos do locatário determinado.  |
|   currentScore    |   Duplo  |   Pontuação atual do locatário obtido na data especificada.    |
|   maxScore |  Duplo  |   Pontuação máxima possível do locatário na data especificada.    |
|   enabledServices |   Coleção de cadeias de caracteres   |   Serviços fornecidos pela Microsoft para o locatário (por exemplo, Exchange Online, Skype, Sharepoint).   |
|   averageComparativeScores |  [coleção averageComparativeScore](averagecomparativescore.md)    |Pontuação média por escopos diferentes (por exemplo, média por setor, média por assento) e categoria de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura) dentro do escopo. |
|   controlScores | [Coleção controlScore](controlscore.md)  |   Contém pontuações de locatário para um conjunto de controles.   |


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



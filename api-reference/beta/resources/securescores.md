---
title: tipo de recurso de secureScores
description: 'superior = n, onde n = o número de dias de dados que você deseja recuperar. '
ms.openlocfilehash: 96d5c487bb854559b0128d93ea8e0783fcc61f0c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033980"
---
# <a name="securescores-resource-type"></a>tipo de recurso de secureScores

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa a pontuação seguro de um locatário por dia da pontuação de dados, no nível de locatário e controle. Por padrão, 90 dias de dados é mantido. Esses dados são classificados pelo **createdDateTime**, do mais recente à mais antiga. Isso permitirá que você para respostas da página usando $top = n, onde n = o número de dias de dados que você deseja recuperar. 


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Lista secureScores](../api/securescores-list.md) | [secureScores](securescores.md) |Leia as propriedades e os metadados de um objeto secureScores.|


## <a name="properties"></a>Propriedades
Propriedades que contêm de tipo de entidade de segurança locatário pontuação (dados diários de instantâneo).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|   azureTenantId   |   String  |   ID de cadeia de caracteres do GUID para o inquilino.  |
|   createdDateTime |   DateTimeOffset  |   A data em que a entidade é criada.  |
|   id  |   String  |   Combinação de azureTenantId_createdDateTime.   |
|   licensedUserCount   |   Int32   |   Licenciado contagem de usuários do determinado inquilino.    |
|   activeUserCount |   Int32   |   Contagem de usuário ativo do determinado inquilino.  |
|   currentScore    |   Duplo  |   Pontuação de locatário atual que já alcançou na data especificada.    |
|   maxScore |  Duplo  |   Locatário pontuação possíveis máxima na data especificada.    |
|   enabledServices |   String collection   |   Serviços fornecida pela Microsoft para o locatário (por exemplo, Exchange online, Skype, Sharepoint).   |
|   averageComparativeScores |  coleção [averageComparativeScore](averagecomparativescore.md)    |Pontuação média por escopos diferentes (por exemplo, média por setor, média por assentos) e a categoria de controle (identidade, dados, dispositivo, aplicativos, infra-estrutura) dentro do escopo. |
|   controlScores | coleção [controlScore](controlscore.md)  |   Contém as pontuações de locatário de um conjunto de controles.   |


## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
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
}

```


<!-- {
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

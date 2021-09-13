---
title: Tipo de recurso secureScore
description: Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível de locatário e controle.
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 01499bbd755739310bc309656379bde278401544
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084122"
---
# <a name="securescore-resource-type"></a>Tipo de recurso secureScore

Namespace: microsoft.graph

Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível de locatário e controle. Por padrão, 90 dias de dados são mantidos. Esses dados são organizados por **createdDateTime**, do mais recente ao mais antigo. Isso permitirá que você page responses by using $top=n, where n = the number of days of data that you want to retrieve. 


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Lista secureScores](../api/security-list-securescores.md) | [Coleção secureScores](securescore.md) |Obter coleção de objetos secureScore.|
|[Obter secureScore](../api/securescore-get.md) | [secureScore](securescore.md) |Ler propriedades e metadados de um objeto secureScore. | 



## <a name="properties"></a>Propriedades

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|id |String|Identificador GUID/exclusivo gerado pelo provedor. Somente leitura. Obrigatório.|
|   azureTenantId   |   String  |   Cadeia de caracteres GUID para ID de locatário.  |
|   activeUserCount |   Int32   |   Contagem ativa do usuário do locatário determinado.  |
|   createdDateTime |   DateTimeOffset  |   A data em que a entidade é criada.  |
|   currentScore    |   Duplo  |   Pontuação atual atingida pelo locatário na data especificada.    |
|   enabledServices |   Coleção String   |   Serviços fornecidos pela Microsoft para o locatário (por exemplo, Exchange online, Skype, Sharepoint).   |
|   licensedUserCount   |   Int32   |   Contagem de usuários licenciados do locatário determinado.    |
|   maxScore |  Duplo  |   Pontuação máxima possível do locatário na data especificada.    |
|   averageComparativeScores |  [Coleção averageComparativeScore](averagecomparativescore.md)    |Pontuação média por escopos diferentes (por exemplo, média por setor, média por assento) e categoria de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura) dentro do escopo. |
|   controlScores | [Coleção controlScore](controlscore.md)  |   Contém pontuações de locatários para um conjunto de controles.   |
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|Tipo complexo que contém detalhes sobre o fornecedor de produtos/serviços de segurança, provedor e subprovider (por exemplo, vendor=Microsoft; provider=SecureScore). Obrigatório.|


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
"id": "String (identifier)",
"azureTenantId": "String",
"activeUserCount": "Int32",
"createdDateTime": "String (timestamp)",
"currentScore": "Double",
"enabledServices": ["String"],
"licensedUserCount": "Int32",
"maxScore": "Double",
"averageComparativeScores": [{"@odata.type": "microsoft.graph.averageComparativeScore"}],
"controlScores": [{"@odata.type": "microsoft.graph.controlScore"}],
"vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


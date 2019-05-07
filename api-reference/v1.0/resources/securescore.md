---
title: tipo de recurso secureScore
description: Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível do locatário e do controle.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 89842579457365f7da10509b2b4ade31f55de4f9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629261"
---
# <a name="securescore-resource-type"></a>tipo de recurso secureScore

Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível do locatário e do controle. Por padrão, são mantidos 90 dias de dados. Esses dados são classificados por **createdDateTime**, do mais recente para o mais antigo. Isso permitirá respostas de página usando $top = n, onde n = o número de dias de dados que você deseja recuperar. 


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Lista secureScores](../api/security-list-securescores.md) | coleção [secureScores](securescore.md) |Obtém a coleção de objetos secureScore.|
|[Obter secureScore](../api/securescore-get.md) | [secureScore](securescore.md) |Leia as propriedades e os metadados de um objeto secureScore. | 



## <a name="properties"></a>Propriedades

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|id |Cadeia de caracteres|Identificador GUID/exclusivo gerado pelo provedor. Somente leitura. Obrigatório.|
|   azureTenantId   |   String  |   Cadeia de caracteres GUID para ID do locatário.  |
|   activeUserCount |   Int32   |   Contagem de usuários ativos de um determinado locatário.  |
|   createdDateTime |   DateTimeOffset  |   A data em que a entidade é criada.  |
|   currentScore    |   Duplo  |   Pontuação Obtida de locatário atual em data especificada.    |
|   enabledservices |   Coleção de cadeias de caracteres   |   Serviços fornecidos pela Microsoft para o locatário (por exemplo, Exchange Online, Skype, SharePoint).   |
|   licensedUserCount   |   Int32   |   Contagem de usuários licenciados de um determinado locatário.    |
|   maxScore |  Duplo  |   Pontuação máxima possível de locatário na data especificada.    |
|   averageComparativeScores |  coleção [averageComparativeScore](averagecomparativescore.md)    |Pontuação média por escopos diferentes (por exemplo, média por setor, média por meio de assentos) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura) dentro do escopo. |
|   controlScores | coleção [controlScore](controlscore.md)  |   Contém pontuações de locatários para um conjunto de controles.   |
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|Tipo complexo que contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = SecureScore). Obrigatório.|


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

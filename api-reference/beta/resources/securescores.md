---
title: tipo de recurso de secureScores
description: 'superior = n, onde n = o número de dias de dados que você deseja recuperar. '
localization_priority: Normal
ms.openlocfilehash: fef5c43130aecf1604677d07f785a0cee0539568
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576077"
---
# <a name="securescores-resource-type"></a>tipo de recurso de secureScores

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|   vendorInformation | [securityVendorInformation](securityvendorinformation.md) | Contém detalhes sobre o fornecedor de serviço do produto de segurança, o provedor e subprovider (por exemplo, o fornecedor = Microsoft; provider = ATP do Windows Defender; subProvider = AppLocker).|

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
    "azureTenantId": "String (identifier)",
    "createdDateTime": "DateTimeOffset",
    "licensedUserCount": "Int32",
    "activeUserCount": "Int32",
    "currentScore": "Double",
    "maxScore": "Double",    
    "enabledServices": ["String"],
    "averageComparativeScores": [{ "@odata.type":"microsoft.graph.averageComparativeScores"}],
    "controlScores": [{"@odata.type":"microsoft.graph.controlScores"}],
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
}
```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescores.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: tipo de recurso secureScoreControlProfiles
description: Representa a pontuação segura de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549171"
---
# <a name="securescorecontrolprofiles-resource-type"></a>tipo de recurso secureScoreControlProfiles

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a pontuação segura de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Lista secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfiles](securescorecontrolprofiles.md) |Leia as propriedades e os metadados de um objeto secureScoreControlProfiles.|


## <a name="properties"></a>Propriedades

|Nome |Tipo |Descrição |
|:--|:--|:--|
|   azureTenantId   |   String  |   Cadeia de caracteres GUID para ID do locatário.  |
|   controlName |   String  |   Nome do controle. |
|   title   |   String  |   Título do controle.   |
| complianceInformation | coleção [complianceInformation](complianceinformation.md) | O conjunto de informações de conformidade associadas ao controle de Pontuação segura |
|   controlCategory |   String  |   Categoria de ação de controle (conta, dados, dispositivo, aplicativos, infraestrutura).  |
|   actionType  |   Cadeia de caracteres  |   Tipo de ação de controle (configuração, revisão, comportamento). |
|   service |   String  |   Serviço que possui o controle (Exchange, SharePoint, Azure AD). |
|   maxScore |  String  |   A pontuação máxima obtida na data especificada.   |
|   camada |  String  |   Camada de controle (Core, defesa profunda, avançada)    |
|   userImpact |    String  | Impacto do usuário da implementação do controle (baixo, moderado, alto).    |
|   implementationCost |    String  |   Custo do recurso do controle implemmentating (baixo, moderado, alto). |
|   classificação |  Int32   |   Classificação de pilha da Microsoft de controle.   |
|   las |   String Collection   |   Lista de ameaças o controle atenua (accountBreach, dataExclusão, dataExfiltration, dataDerramamento, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, falsificação). |
|   preterido |    Booliano |   Sinalizador para indicar se um controle está depreciado.   |
|   correção |   String  |   Descrição do que o controle ajudará a corrigir. |
|   remediationImpact | String  |   Descrição do impacto sobre os usuários da correção. |
|   actionUrl | String  |   URL para onde o controle pode ser acionado. |
|   controlStateUpdates |   coleção [secureScoreControlStateUpdate](securescorecontrolstateupdate.md) |    Sinalizador para indicar onde o locatário marcou um controle (ignore, terceiros, revisado) (suporta [atualização](../api/securescorecontrolprofiles-update.md)). |

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
"title": "String", 
"azureTenantId": "Guid", 
"referenceId": "String", 
"controlName": "String", 
"maxScore": "Int32",
"actionCategory": "Collection(microsoft.graph.SecureScore.actionCategory)",
"actionType": "Collection(microsoft.graph.SecureScore.actionType)",
"service": "String",
"tier": "Collection(microsoft.graph.SecureScore.tier)",
"userImpact": "Collection(microsoft.graph.SecureScore.ranking)",
"implementationCost ": "Collection(microsoft.graph.SecureScore.ranking)",
"rank ": "Int32",
"threats": "Collection(microsoft.graph.SecureScore.threat)",
"deprecated ": "Boolean",
"remediation": "String",
"remediationImpact ": "String",
"actionUrl": "String",
"controlStateUpdates": "Collection(microsoft.graph.SecureScore.controlStateUpdates)",
"tenantNotes": "String",
"upn": "String",
"comments": "String",
}


```


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescorecontrolprofiles.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

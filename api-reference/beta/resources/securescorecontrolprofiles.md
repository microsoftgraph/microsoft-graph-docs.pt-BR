---
title: tipo de recurso secureScoreControlProfile
description: Representa a pontuação segura de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.
localization_priority: Normal
ms.openlocfilehash: 41a74af0de47bbe77b8ea04cbea011a6f085d1bb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343406"
---
# <a name="securescorecontrolprofile-resource-type"></a>tipo de recurso secureScoreControlProfile

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a pontuação segura de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Lista secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | coleção [secureScoreControlProfile](securescorecontrolprofiles.md) |Obtenha uma coleção de objetos secureScoreControlProfile.|


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
|   preterido |    Boolean |   Sinalizador para indicar se um controle está depreciado.   |
|   correção |   String  |   Descrição do que o controle ajudará a corrigir. |
|   remediationImpact | String  |   Descrição do impacto sobre os usuários da correção. |
|   actionUrl | String  |   URL para onde o controle pode ser acionado. |
|   controlStateUpdates | coleção [secureScoreControlStateUpdate](securescorecontrolstateupdate.md) |    Sinalizador para indicar onde o locatário marcou um controle (ignore, terceiros, revisado) (suporta [atualização](../api/securescorecontrolprofiles-update.md)). |
|   vendorInformation | [securityVendorInformation](securityvendorinformation.md) |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}-->

```json
{
  "title": "String",
  "azureTenantId": "String (identifier)",
  "maxScore": 1024.13,
  "actionType": "String",
  "service": "String",
  "tier": "String",
  "userImpact": "string",
  "implementationCost ": "String",
  "rank ": 100,
  "threats": ["string"],
  "deprecated ": false,
  "remediation": "String",
  "remediationImpact ": "String",
  "actionUrl": "String",
  "controlStateUpdates": [{"@odata.type": "microsoft.graph.secureScoreControlStateUpdate"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
  "complianceInformation": [{"@odata.type": "microsoft.graph.complianceInformation"}],
  "controlCategory": "string",
  "lastModifiedDateTime": "String (timestamp)"
}


```


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

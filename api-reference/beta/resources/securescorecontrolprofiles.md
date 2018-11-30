---
title: tipo de recurso de secureScoreControlProfiles
description: Representa a pontuação seguro de um locatário por dados do controle. Por padrão, ela retorna todos os controles para um inquilino e explicitamente pode extrair controles individuais.
ms.openlocfilehash: e02c9ae3b1431b131576e2e0e115377dd3480bc2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038542"
---
# <a name="securescorecontrolprofiles-resource-type"></a>tipo de recurso de secureScoreControlProfiles

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa a pontuação seguro de um locatário por dados do controle. Por padrão, ela retorna todos os controles para um inquilino e explicitamente pode extrair controles individuais.


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Lista secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfiles](securescorecontrolprofiles.md) |Leia as propriedades e os metadados de um objeto secureScoreControlProfiles.|


## <a name="properties"></a>Propriedades

|Nome |Tipo |Descrição |
|:--|:--|:--|
|   azureTenantId   |   String  |   ID de cadeia de caracteres do GUID para o inquilino.  |
|   controlName |   String  |   Nome do controle. |
|   title   |   String  |   Título do controle.   |
|   controlCategory |   String  |   Categoria de ação de controle (conta, dados, dispositivo, aplicativos, infra-estrutura).  |
|   actionType  |   Cadeia de caracteres  |   Controlar o tipo de ação (Config, revisão, comportamento). |
|   service |   String  |   Serviço que possui o controle (Exchange, Sharepoint, Azure AD). |
|   maxScore |  String  |   Atual obtidos max pontuação na data especificada.   |
|   camada |  String  |   Camada de controle (Core, defesa em camadas, avançadas.)    |
|   userImpact |    String  | Impacto da implementação de controle (baixa, moderada, alta) do usuário.    |
|   implementationCost |    String  |   Custo do recurso de controle de implemmentating (baixa, moderada, alta). |
|   rank |  Int32   |   Pilha da Microsoft de classificação do controle.   |
|   ameaças |   Coleção de cadeia de caracteres   |   Lista de ameaças reduz o controle (accountBreach, dataDeletion, dataExfiltration, dataSpillage, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, falsificação). |
|   preteridos |    Booliano |   Sinalizador para indicar se um controle é depreciado.   |
|   remediação |   String  |   Descrição do controle que ajudarão remediar. |
|   remediationImpact | String  |   Descrição do impacto sobre os usuários da remediação. |
|   actionUrl | String  |   URL para o qual o controle pode ser actioned. |
|   controlStateUpdates |   String  |   Sinalizador para indicar onde o inquilino tenha marcado a um controle (Ignorar, thirdParty, examinado) (oferece suporte a [atualização](../api/securescorecontrolprofiles-update.md)). |
|   tenantNote |    String  |   Inquilino pode ser definida por comentários do controle (suporta a [atualização](../api/securescorecontrolprofiles-update.md)). |
|   assignedTo |    String  |   Inquilino pode atribuir o controle a um indivíduo (suporta a [atualização](../api/securescorecontrolprofiles-update.md)). |
|   updatedBy | String  |   Nome principal do usuário de quem fez as alterações para o estado de um controle. |

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


<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

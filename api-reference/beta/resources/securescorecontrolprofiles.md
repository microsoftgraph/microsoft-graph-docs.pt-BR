---
title: tipo de recurso de secureScoreControlProfiles
description: Representa a pontuação seguro de um locatário por dados do controle. Por padrão, ela retorna todos os controles para um inquilino e explicitamente pode extrair controles individuais.
localization_priority: Normal
ms.openlocfilehash: 866b2086ff5160744f848292cedf30c3cedf6daa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866217"
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
|   azureTenantId   |   Cadeia de caracteres  |   ID de cadeia de caracteres do GUID para o inquilino.  |
|   controlName |   Cadeia de caracteres  |   Nome do controle. |
|   title   |   Cadeia de caracteres  |   Título do controle.   |
| complianceInformation | coleção [complianceInformation](complianceinformation.md) | A coleção de informações de conformidade associadas a proteger o controle de pontuação |
|   controlCategory |   Cadeia de caracteres  |   Categoria de ação de controle (conta, dados, dispositivo, aplicativos, infra-estrutura).  |
|   actionType  |   Cadeia de caracteres  |   Controlar o tipo de ação (Config, revisão, comportamento). |
|   service |   Cadeia de caracteres  |   Serviço que possui o controle (Exchange, Sharepoint, Azure AD). |
|   maxScore |  Cadeia de caracteres  |   Atual obtidos max pontuação na data especificada.   |
|   camada |  Cadeia de caracteres  |   Camada de controle (Core, defesa em camadas, avançadas.)    |
|   userImpact |    Cadeia de caracteres  | Impacto da implementação de controle (baixa, moderada, alta) do usuário.    |
|   implementationCost |    Cadeia de caracteres  |   Custo do recurso de controle de implemmentating (baixa, moderada, alta). |
|   rank |  Int32   |   Pilha da Microsoft de classificação do controle.   |
|   ameaças |   Coleção de cadeia de caracteres   |   Lista de ameaças reduz o controle (accountBreach, dataDeletion, dataExfiltration, dataSpillage, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, falsificação). |
|   preteridos |    Booliano |   Sinalizador para indicar se um controle é depreciado.   |
|   remediação |   Cadeia de caracteres  |   Descrição do controle que ajudarão remediar. |
|   remediationImpact | Cadeia de caracteres  |   Descrição do impacto sobre os usuários da remediação. |
|   actionUrl | Cadeia de caracteres  |   URL para o qual o controle pode ser actioned. |
|   controlStateUpdates |   coleção [secureScoreControlStateUpdate](securescorecontrolstateupdate.md) |    Sinalizador para indicar onde o inquilino tenha marcado a um controle (Ignorar, thirdParty, examinado) (oferece suporte a [atualização](../api/securescorecontrolprofiles-update.md)). |

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

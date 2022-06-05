---
title: Tipo de recurso secureScoreControlProfile
description: Representa a pontuação de segurança de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode efetuar pull explícito de controles individuais.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: dd4e9ee6372e9d063515ad83e851008e01ec6b60
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900139"
---
# <a name="securescorecontrolprofile-resource-type"></a>Tipo de recurso secureScoreControlProfile

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a pontuação de segurança de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode efetuar pull explícito de controles individuais.


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Lista secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [coleção secureScoreControlProfile](securescorecontrolprofiles.md) |Obtenha uma coleção de objetos secureScoreControlProfile.|


## <a name="properties"></a>Propriedades

|Nome |Tipo |Descrição |
|:--|:--|:--|
|   azureTenantId   |   String  |   Cadeia de caracteres GUID para a ID do locatário.  |
|   Controlname |   Cadeia de Caracteres  |   Nome do controle. |
|   title   |   String  |   Título do controle.   |
| complianceInformation | [coleção complianceInformation](complianceinformation.md) | A coleção de informações de conformidade associadas ao controle de pontuação segura |
|   controlCategory |   Cadeia de Caracteres  |   Categoria de ação de controle (Conta, Dados, Dispositivo, Aplicativos, Infraestrutura).  |
|   actionType  |   Cadeia de caracteres  |   Tipo de ação de controle (Configuração, Revisão, Comportamento). |
|   service |   Cadeia de caracteres  |   Serviço que possui o controle (Exchange, Sharepoint, Azure AD). |
|   maxScore |  Cadeia de Caracteres  |   Pontuação máxima obtida no momento na data especificada.   |
|   Camada |  Cadeia de Caracteres  |   Camada de controle (Core, Defesa em Profundidade, Avançado.)    |
|   userImpact |    Cadeia de Caracteres  | Impacto do usuário na implementação do controle (baixo, moderado, alto).    |
|   implementationCost |    Cadeia de Caracteres  |   Custo de recurso de controle implemmentating (baixo, moderado, alto). |
|   classificação |  Int32   |   Classificação de pilha da Microsoft de controle.   |
|   Ameaças |   String Collection   |   Lista de ameaças que o controle reduz (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing). |
|   Preterido |    Booliano |   Sinalizador para indicar se um controle é depreciado.   |
|   Remediação |   String  |   Descrição do que o controle ajudará a corrigir. |
|   remediationImpact | Cadeia de Caracteres  |   Descrição do impacto sobre os usuários da correção. |
|   Actionurl | Cadeia de Caracteres  |   URL para onde o controle pode ser acionado. |
|   controlStateUpdates | [coleção secureScoreControlStateUpdate](securescorecontrolstateupdate.md) |    Sinalizador para indicar onde o locatário marcou um controle (ignorar, thirdParty, revisado) (dá suporte à [atualização](../api/securescorecontrolprofiles-update.md)). |
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



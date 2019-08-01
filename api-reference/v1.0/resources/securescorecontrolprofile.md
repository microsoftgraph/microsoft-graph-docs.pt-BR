---
title: tipo de recurso secureScoreControlProfile
description: Representa a pontuação segura de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 40bee951d3030772973911510ebba7cc90f412ae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034486"
---
# <a name="securescorecontrolprofile-resource-type"></a>tipo de recurso secureScoreControlProfile

Representa a pontuação segura de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Lista secureScoreControlProfiles](../api/security-list-securescorecontrolprofiles.md) | [secureScoreControlProfile](securescorecontrolprofile.md) |Leia as propriedades e os metadados de um objeto secureScoreControlProfiles.|
|[Obter secureScoreControlProfile](../api/securescorecontrolprofile-get.md) | [securescorecontrolprofile](securescorecontrolprofile.md) |Leia as propriedades e os metadados de um objeto secureScoreControlProfiles.|
|[Atualizar securescorecontrolprofile](../api/securescorecontrolprofile-update.md) | [securescorecontrolprofile](securescorecontrolprofile.md) |Atualize um objeto securescorecontrolprofile. |


## <a name="properties"></a>Propriedades

|Nome |Tipo |Descrição |
|:--|:--|:--|
|id|String|Identificador GUID/exclusivo gerado pelo provedor. Somente leitura. Obrigatório.|
|azureTenantId|String|Cadeia de caracteres GUID para ID do locatário.|
|actionType|Cadeia de caracteres|Tipo de ação de controle (configuração, revisão, comportamento).|
|actionUrl|String|URL para onde o controle pode ser acionado. |
|controlCategory|String|Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).|
|title|String|Título do controle.|
|preterido|Booliano|Sinalizador para indicar se um controle está depreciado.|
|implementationCost|String|Custo do recurso do controle implemmentating (baixo, moderado, alto).|
|lastModifiedDateTime|DateTimeOffset|Hora em que a entidade de perfil de controle foi modificada pela última vez. O tipo TIMESTAMP representa data e hora| 
|maxScore|Duplo|Pontuação máxima atingível do controle.|
|classificação|Int32|Classificação de pilha da Microsoft de controle.|
|correção|String|Descrição do que o controle ajudará a corrigir.|
|remediationImpact|String|Descrição do impacto sobre os usuários da correção.|
|service|String|Serviço que possui o controle (Exchange, SharePoint, Azure AD).|
|las|Coleção de cadeias de caracteres|Lista de ameaças que o controle atenua (accountBreach, dataexclusão, dataExfiltration, dataderramamento
elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, falsificação).|
|camada|String|Camada de controle (Core, defesa profunda, avançada)   |
|userimpact|String|Impacto do usuário da implementação do controle (baixo, moderado, alto).   |
|complianceInformation|coleção [complianceInformation](complianceinformation.md)|O conjunto de informações de conformidade associadas ao controle de Pontuação segura|
|controlStateUpdates|coleção [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)|Sinalizador para indicar onde o locatário marcou um controle (ignorado, terceiros, revisado) (suporta [atualização](../api/securescorecontrolprofile-update.md)).|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|Tipo complexo que contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = SecureScore). Obrigatório.|

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
  "id": "String (identifier)",
  "azureTenantId": "String",
  "actionType": "String",
  "actionUrl": "String",
  "controlCategory": "String",
  "title": "String", 
  "deprecated": "Boolean",
  "implementationCost": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "maxScore": "Double",
  "rank": "Int32",
  "remediation": "String",
  "remediationImpact": "String",
  "service": "String",
  "threats": ["String"],
  "tier": "String",
  "userImpact": "String",
  "complianceInformation": [{"@odata.type": "microsoft.graph.complianceInformation"}], 
  "controlStateUpdates": [{"@odata.type": "microsoft.graph.secureScoreControlStateUpdate"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

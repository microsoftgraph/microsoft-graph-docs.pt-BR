---
title: Tipo de recurso secureScoreControlProfile
description: Representa a pontuação de segurança de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode efetuar pull explícito de controles individuais.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6c54901018dcb6eccf36be2f6f4b0fc1c7d9da8d
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899831"
---
# <a name="securescorecontrolprofile-resource-type"></a>Tipo de recurso secureScoreControlProfile

Namespace: microsoft.graph

Representa a pontuação de segurança de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode efetuar pull explícito de controles individuais.


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Lista secureScoreControlProfiles](../api/security-list-securescorecontrolprofiles.md) | [secureScoreControlProfile](securescorecontrolprofile.md) |Ler propriedades e metadados de um objeto secureScoreControlProfiles.|
|[Obter secureScoreControlProfile](../api/securescorecontrolprofile-get.md) | [securescorecontrolprofile](securescorecontrolprofile.md) |Ler propriedades e metadados de um objeto secureScoreControlProfiles.|
|[Atualizar securescorecontrolprofile](../api/securescorecontrolprofile-update.md) | [securescorecontrolprofile](securescorecontrolprofile.md) |Atualize um objeto securescorecontrolprofile. |


## <a name="properties"></a>Propriedades

|Nome |Tipo |Descrição |
|:--|:--|:--|
|id|String|Identificador GUID/exclusivo gerado pelo provedor. Somente leitura. Obrigatório.|
|azureTenantId|String|Cadeia de caracteres GUID para a ID do locatário.|
|actionType|Cadeia de caracteres|Tipo de ação de controle (Configuração, Revisão, Comportamento).|
|Actionurl|Cadeia de Caracteres|URL para onde o controle pode ser acionado. |
|controlCategory|Cadeia de Caracteres|Categoria de ação de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura).|
|title|String|Título do controle.|
|Preterido|Booliano|Sinalizador para indicar se um controle é depreciado.|
|implementationCost|Cadeia de Caracteres|Custo de recurso de controle implemmentating (baixo, moderado, alto).|
|lastModifiedDateTime|DateTimeOffset|Hora em que a entidade de perfil de controle foi modificada pela última vez. O tipo de carimbo de data/hora representa a data e a hora| 
|maxScore|Duplo|pontuação máxima alcançável para o controle.|
|classificação|Int32|Classificação de pilha da Microsoft de controle.|
|Remediação|String|Descrição do que o controle ajudará a corrigir.|
|remediationImpact|Cadeia de Caracteres|Descrição do impacto sobre os usuários da correção.|
|service|Cadeia de caracteres|Serviço que possui o controle (Exchange, Sharepoint, Azure AD).|
|Ameaças|Coleção de cadeias de caracteres|Lista de ameaças que o controle reduz (accountBreach,dataDeletion,dataExfiltration,dataSpillage,
elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).|
|Camada|Cadeia de Caracteres|Camada de controle (Core, Defesa em Profundidade, Avançado.)   |
|userImpact|Cadeia de Caracteres|Impacto do usuário na implementação do controle (baixo, moderado, alto).   |
|complianceInformation|[coleção complianceInformation](complianceinformation.md)|A coleção de informações de conformidade associadas ao controle de pontuação segura|
|controlStateUpdates|[coleção secureScoreControlStateUpdate](securescorecontrolstateupdate.md)|Sinalizador para indicar onde o locatário marcou um controle (ignorado, thirdParty, revisado) (dá suporte à [atualização](../api/securescorecontrolprofile-update.md)).|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|Tipo complexo que contém detalhes sobre o fornecedor, o provedor e o subprovidador de produto/serviço de segurança (por exemplo, vendor=Microsoft; provider=SecureScore). Obrigatório.|

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


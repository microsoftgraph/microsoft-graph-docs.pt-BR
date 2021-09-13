---
title: Tipo de recurso secureScoreControlProfile
description: Representa a pontuação segura de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode puxar explicitamente controles individuais.
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 856ed0ca50a2aadb6945f5213de2f4b0f9ac286a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084101"
---
# <a name="securescorecontrolprofile-resource-type"></a>Tipo de recurso secureScoreControlProfile

Namespace: microsoft.graph

Representa a pontuação segura de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode puxar explicitamente controles individuais.


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Lista secureScoreControlProfiles](../api/security-list-securescorecontrolprofiles.md) | [secureScoreControlProfile](securescorecontrolprofile.md) |Leia propriedades e metadados de um objeto secureScoreControlProfiles.|
|[Obter secureScoreControlProfile](../api/securescorecontrolprofile-get.md) | [securescorecontrolprofile](securescorecontrolprofile.md) |Leia propriedades e metadados de um objeto secureScoreControlProfiles.|
|[Atualizar securescorecontrolprofile](../api/securescorecontrolprofile-update.md) | [securescorecontrolprofile](securescorecontrolprofile.md) |Atualize um objeto securescorecontrolprofile. |


## <a name="properties"></a>Propriedades

|Nome |Tipo |Descrição |
|:--|:--|:--|
|id|String|Identificador GUID/exclusivo gerado pelo provedor. Somente leitura. Obrigatório.|
|azureTenantId|String|Cadeia de caracteres GUID para ID de locatário.|
|actionType|Cadeia de caracteres|Tipo de ação de controle (Config, Review, Behavior).|
|actionUrl|String|URL para onde o controle pode ser a ação. |
|controlCategory|Cadeia de caracteres|Categoria de ação de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura).|
|title|String|Título do controle.|
|preterido|Booliano|Sinalizador para indicar se um controle é depreciado.|
|implementationCost|Cadeia de caracteres|Custo de recurso do controle implemmentating (baixo, moderado, alto).|
|lastModifiedDateTime|DateTimeOffset|Hora em que a entidade de perfil de controle foi modificada pela última vez. O tipo Timestamp representa data e hora| 
|maxScore|Duplo|pontuação máxima possível para o controle.|
|classificação|Int32|Classificação de pilha da Microsoft de controle.|
|correção|Cadeia de caracteres|Descrição do que o controle ajudará a correção.|
|remediationImpact|String|Descrição do impacto nos usuários da correção.|
|service|Cadeia de caracteres|Serviço que possui o controle (Exchange, Sharepoint, Azure AD).|
|threats|Coleção String|Lista de ameaças que o controle reduz (accountBreach,dataDeletion,dataExfiltration,dataSpillage,
elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).|
|tier|Cadeia de caracteres|Camada de controle (Core, Defense in Depth, Advanced.)   |
|userImpact|Cadeia de caracteres|Impacto do usuário na implementação do controle (baixo, moderado, alto).   |
|complianceInformation|[Coleção complianceInformation](complianceinformation.md)|A coleção de informações de conformidade associadas ao controle de pontuação seguro|
|controlStateUpdates|[Coleção secureScoreControlStateUpdate](securescorecontrolstateupdate.md)|Sinalizador para indicar onde o locatário marcou um controle (ignorado, thirdParty, revisado) (suporta [atualização](../api/securescorecontrolprofile-update.md)).|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|Tipo complexo que contém detalhes sobre o fornecedor de produtos/serviços de segurança, provedor e subprovider (por exemplo, vendor=Microsoft; provider=SecureScore). Obrigatório.|

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


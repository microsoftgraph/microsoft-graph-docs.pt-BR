---
title: tipo de recurso de secureScoreControlProfiles
description: Representa a pontuação seguro de um locatário por dados do controle. Por padrão, ela retorna todos os controles para um inquilino e explicitamente pode extrair controles individuais.
localization_priority: Normal
ms.openlocfilehash: 4e599bbffd291de51ba478f8661999d01c8c8998
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576056"
---
# <a name="securescorecontrolprofiles-resource-type"></a>tipo de recurso de secureScoreControlProfiles

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a pontuação seguro de um locatário por dados do controle. Por padrão, ela retorna todos os controles para um inquilino e explicitamente pode extrair controles individuais.


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Lista secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfile](securescorecontrolprofiles.md) |Leia as propriedades e os metadados de um objeto secureScoreControlProfiles.|


## <a name="properties"></a>Propriedades

|Nome |Tipo |Descrição |
|:--|:--|:--|
|   azureTenantId   |   String  |   ID de cadeia de caracteres do GUID para o inquilino.  |
|   controlName |   String  |   Nome do controle. |
|   title   |   String  |   Título do controle.   |
|   controlCategory |   String  |   Categoria de ação de controle (conta, dados, dispositivo, aplicativos, infra-estrutura).  |
|   actionType  |   Cadeia de caracteres  |   Controlar o tipo de ação (Config, revisão, comportamento). |
|   service |   String  |   Serviço que possui o controle (Exchange, Sharepoint, Azure AD). |
|   maxScore |  Duplo  |   Atual obtidos max pontuação na data especificada.   |
|   camada |  String  |   Camada de controle (Core, defesa em camadas, avançadas.)    |
|   userImpact |    String  | Impacto da implementação de controle (baixa, moderada, alta) do usuário.    |
|   implementationCost |    String  |   Custo do recurso de controle de implemmentating (baixa, moderada, alta). |
|   rank |  Int32   |   Pilha da Microsoft de classificação do controle.   |
|   ameaças |   Coleção de cadeia de caracteres   |   Lista de ameaças reduz o controle (accountBreach, dataDeletion, dataExfiltration, dataSpillage, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, falsificação). |
|   preteridos |    Boolean |   Sinalizador para indicar se um controle é depreciado.   |
|   remediação |   String  |   Descrição do controle que ajudarão remediar. |
|   remediationImpact | String  |   Descrição do impacto sobre os usuários da remediação. |
|   actionUrl | String  |   URL para o qual o controle pode ser actioned. |
|   lastModifiedDateTime |  Cadeia de caracteres (DateTimeOffset) |   Data da última modificada |
|   controlStateUpdates |   coleção [secureScoreControlStateUpdate](securescorecontrolstateupdate.md) |  Sinalizador para indicar onde o inquilino tenha marcado a um controle (Ignorar, thirdParty, examinado) (oferece suporte a [atualização](../api/securescorecontrolprofiles-update.md)). |
|   vendorInformation | [securityVendorInformation](securityvendorinformation.md) | Contém detalhes sobre o fornecedor de serviço do produto de segurança, o provedor e subprovider (por exemplo, o fornecedor = Microsoft; provider = ATP do Windows Defender; subProvider = AppLocker).|

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
    "referenceId": "String", 
    "controlName": "String", 
    "maxScore": "Double",
    "controlCategory": "string",
    "actionType": "string",
    "service": "String",
    "tier": "string",
    "userImpact": "string",
    "implementationCost ": "string",
    "rank ": "Int32",
    "deprecated ": "Boolean",
    "remediation": "String",
    "remediationImpact ": "String",
    "actionUrl": "String",
    "lastModifiedDateTime": "   String (DateTimeOffset)",
    "controlStateUpdates": [{"odata.type":"microsoft.graph.secureScorecontrolStateUpdates"}],
    "tenantNotes": "String",
    "upn": "String",    
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
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

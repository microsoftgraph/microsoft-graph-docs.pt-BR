---
title: tipo de recurso authorizationPolicy
description: Representa uma política que pode controlar as configurações de autorização do Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c20f4dad0263e9d4c931e43da99870ed022f1e58
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492198"
---
# <a name="authorizationpolicy-resource-type"></a>tipo de recurso authorizationPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política que pode controlar as configurações de autorização do Azure Active Directory. É um singleton que herda do tipo de política base e sempre existe para o locatário. 

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter authorizationPolicy](../api/authorizationpolicy-get.md) | [authorizationPolicy](authorizationpolicy.md) | Leia o objeto authorizationPolicy. |
| [Atualizar authorizationPolicy](../api/authorizationpolicy-update.md) | Nenhum | Atualize o objeto authorizationPolicy. |

## <a name="properties"></a>Propriedades  
| Propriedade | Tipo | Descrição | 
|-|-|-|
|id|String| ID da política de autorização. Obrigatório. Somente leitura.| 
|displayName|Cadeia de caracteres| Nome para exibição dessa política. |  
|description|String| Descrição da política.|  
|guestUserRoleId|Guid| Representa o modelo de função para a função que deve ser concedida ao usuário convidado. Consulte [list unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) para encontrar a lista de modelos de função disponíveis. As funções a seguir são suportadas: usuário (a0b1b346-4d3e-4e8b-98f8-753987be4970), usuário convidado (10dae51f-b6af-4016-8d66-8c2a99b929b3) e usuário convidado restrito (2af84b1e-32c8-42b7-82bc-daa82404023b). | 
|enabledPreviewFeatures|Coleção (cadeia de caracteres)| Lista de recursos habilitados para visualização privada no locatário. | 
|blockMsolPowerShell|Booliano| Para desabilitar o uso do MSOL PowerShell defina essa propriedade como true. A configuração como true também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSOL PowerShell. Isso não afeta o Azure AD Connect ou o Microsoft Graph. | 


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authorizationPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
   "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "enabledPreviewFeatures": "[String]",
  "guestUserRoleId": "Guid",
  "blockMsolPowerShell": true 
}
```

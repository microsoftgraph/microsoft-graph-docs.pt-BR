---
title: tipo de recurso authorizationPolicy
description: Representa uma política que pode controlar as configurações de autorização do Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0cc59543d15f9141c8857e653edc7c84ebb692bc
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921547"
---
# <a name="authorizationpolicy-resource-type"></a>tipo de recurso authorizationPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política que pode controlar as configurações de autorização do Azure Active Directory. É um singleton que herda do tipo de política base e sempre existe para o locatário. 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter authorizationPolicy](../api/authorizationpolicy-get.md) | [authorizationPolicy](authorizationpolicy.md) | Leia o objeto authorizationPolicy. |
| [Atualizar authorizationPolicy](../api/authorizationpolicy-update.md) | Nenhum | Atualize o objeto authorizationPolicy. |

## <a name="properties"></a>Propriedades  
| Propriedade | Tipo | Descrição | 
|-|-|-|
|id|String| ID da política de autorização. Obrigatório. Somente leitura.| 
|displayName|String| Nome para exibição dessa política. |  
|description|String| Descrição da política.|  
|guestUserRoleId|Guid| Representa o modelo de função para a função que deve ser concedida ao usuário convidado. Consulte [list unifiedRoleDefinitions](../api/rbacapplication-list-roledefinitions.md) para encontrar a lista de modelos de função disponíveis. As funções a seguir são suportadas: usuário (a0b1b346-4d3e-4e8b-98f8-753987be4970), usuário convidado (10dae51f-b6af-4016-8d66-8c2a99b929b3) e usuário convidado restrito (2af84b1e-32c8-42b7-82bc-daa82404023b). | 
|enabledPreviewFeatures|Coleção de cadeias de caracteres| Lista de recursos habilitados para visualização privada no locatário. | 
|blockMsolPowerShell|Booliano| Para desabilitar o uso do MSOL PowerShell defina essa propriedade como true. A configuração como true também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSOL PowerShell. Isso não afeta o Azure AD Connect ou o Microsoft Graph. | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultUserRolePermissions.md)| Especifica determinadas permissões personalizáveis para a função de usuário padrão. | 
|allowedToUseSSPR|Booliano| Indica se o Self-Serve recurso de redefinição de senha pode ser usado por usuários no locatário. | 
|allowedToSignUpEmailBasedSubscriptions|Booliano| Indica se os usuários podem se inscrever para assinaturas baseadas em email. | 
|allowEmailVerifiedUsersToJoinOrganization|Booliano| Indica se um usuário pode ingressar no locatário por validação de email. | 
|allowInvitesFrom|String|Indica quem pode convidar usuários externos para a organização. Os valores possíveis são:<ul><li>`none` – Impedir que todos, incluindo administradores, convidarem usuários externos. Configuração padrão para o governo dos EUA.</li><li>`adminsAndGuestInviters` – Permitir que membros de administradores globais, administradores de usuários e funções do convidado de convidados convidarem usuários externos.</li><li>`adminsGuestInvitersAndAllMembers` – Permitir que as funções de administrador acima e todos os outros membros da função de usuário convidem usuários externos.</li><li>`everyone` – Permitir que todos na organização, incluindo usuários convidados, convidem usuários externos. Configuração padrão para todos os ambientes de nuvem, exceto o governo dos EUA.</li></ul> |
|permissionGrantPolicyIdsAssignedToDefaultUserRole|Coleção de cadeias de caracteres|Indica se o consentimento do usuário para os aplicativos é permitido e, se for, qual política de consentimento de aplicativos (permissionGrantPolicy) governará a permissão para que os usuários concedam o consentimento. Os valores devem estar no formato `managePermissionGrantsForSelf.{id}` , onde `{id}` é a **ID** de uma [política de consentimento de aplicativo](/azure/active-directory/manage-apps/manage-app-consent-policies)interna ou personalizada. Uma lista vazia indica que o consentimento do usuário para os aplicativos está desabilitado. |

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
  "blockMsolPowerShell": true,
  "defaultUserRolePermissions": {"@odata.type": "microsoft.graph.defaultUserRolePermissions"},
  "allowedToUseSSPR": true,
  "allowedToSignUpEmailBasedSubscriptions": true,
  "allowEmailVerifiedUsersToJoinOrganization": true,
  "allowInvitesFrom": "String",
  "permissionGrantPolicyIdsAssignedToDefaultUserRole": "[String]"
}
```

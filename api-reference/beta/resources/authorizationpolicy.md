---
title: Tipo de recurso authorizationPolicy
description: Representa uma política que pode controlar as configurações de autorização do Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e9ad1a67a2aae2c1af4ffa45dcd85228a4c95f25
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433170"
---
# <a name="authorizationpolicy-resource-type"></a>Tipo de recurso authorizationPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política que pode controlar as configurações de autorização do Azure Active Directory. É um singleton que herda do tipo de política base e sempre existe para o locatário. 

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter authorizationPolicy](../api/authorizationpolicy-get.md) | [authorizationPolicy](authorizationpolicy.md) | Leia o objeto authorizationPolicy. |
| [Atualizar authorizationPolicy](../api/authorizationpolicy-update.md) | Nenhum(a) | Atualize o objeto authorizationPolicy. |

## <a name="properties"></a>Propriedades  
| Propriedade | Tipo | Descrição | 
|-|-|-|
|id|String| ID da política de autorização. Obrigatório. Somente leitura.| 
|displayName|String| Nome de exibição para esta política. |  
|descrição|String| Descrição dessa política.|  
|guestUserRoleId|Guid| Representa modelo de funçãoId para a função que deve ser concedida ao usuário convidado. Consulte [Listar unifiedRoleDefinitions](../api/rbacapplication-list-roledefinitions.md) para encontrar a lista de modelos de função disponíveis. Atualmente, há suporte para funções a seguir: Usuário (a0b1b346-4d3e-4e8b-98f8-753987be4970), Usuário Convidado (10dae51f-b6af-40 16-8d66-8c2a99b929b3) e Usuário Convidado Restrito (2af84b1e-32c8-42b7-82bc-daa82404023b). | 
|enabledPreviewFeatures|Coleção de cadeias de caracteres| Lista de recursos habilitados para visualização privada no locatário. | 
|blockMsolPowerShell|Booliano| Para desabilitar o uso do MSOL PowerShell, de definir essa propriedade como true. A configuração como true também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSOL PowerShell. Isso não afeta o Azure AD Connect ou o Microsoft Graph. | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultUserRolePermissions.md)| Especifica determinadas permissões personalizáveis para a função de usuário padrão. | 
|allowedToUseSSPR|Booliano| Indica se o recurso Self-Serve redefinição de senha pode ser usado pelos usuários no locatário. | 
|allowedToSignUpEmailBasedSubscriptions|Booliano| Indica se os usuários podem se inscrever para assinaturas baseadas em email. | 
|allowEmailVerifiedUsersToJoinOrganization|Booliano| Indica se um usuário pode ingressar no locatário por validação de email. | 
|allowInvitesFrom|String|Indica quem pode convidar usuários externos para a organização. Os valores possíveis são:<ul><li>`none` - Impedir que todos, incluindo administradores, convidam usuários externos. Configuração padrão para o Governo dos EUA.</li><li>`adminsAndGuestInviters` - Permitir que os membros das funções Administradores Globais, Administradores de Usuários e Convidados convidem usuários externos.</li><li>`adminsGuestInvitersAndAllMembers` - Permitir que as funções de administrador acima e todos os outros membros da função de usuário convidem usuários externos.</li><li>`everyone` - Permitir que todos na organização, incluindo usuários convidados, convidem usuários externos. Configuração padrão para todos os ambientes de nuvem, exceto o Governo dos EUA.</li></ul> |
|permissionGrantPolicyIdsAssignedToDefaultUserRole|Coleção de cadeias de caracteres|Indica se o consentimento do usuário para aplicativos é permitido e, se for, qual política de consentimento de aplicativo (permissionGrantPolicy) rege a permissão para que os usuários concedam consentimento. Os valores devem estar no formato `managePermissionGrantsForSelf.{id}` , onde é a id de uma política de consentimento de aplicativo interna ou `{id}` [personalizada.](/azure/active-directory/manage-apps/manage-app-consent-policies)  Uma lista vazia indica que o consentimento do usuário para aplicativos está desabilitado. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authorizationPolicy",
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

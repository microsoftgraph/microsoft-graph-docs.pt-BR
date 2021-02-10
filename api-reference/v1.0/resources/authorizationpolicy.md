---
title: Tipo de recurso authorizationPolicy
description: Representa uma política que pode controlar as configurações de autorização do Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 12fe4ad670d2bb5056d05fde533d4b690068f7a5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154212"
---
# <a name="authorizationpolicy-resource-type"></a>Tipo de recurso authorizationPolicy

Namespace: microsoft.graph

Representa uma política que pode controlar as configurações de autorização do Azure Active Directory. É um singleton que herda do tipo de política base e sempre existe para o locatário.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter authorizationPolicy](../api/authorizationpolicy-get.md) | [authorizationPolicy](authorizationpolicy.md) | Leia o objeto authorizationPolicy. |
| [Atualizar authorizationPolicy](../api/authorizationpolicy-update.md) | Nenhum | Atualize o objeto authorizationPolicy. |

## <a name="properties"></a>Propriedades  
| Propriedade | Tipo | Descrição | 
|-|-|-|
|id|Cadeia de caracteres| ID da política de autorização. Obrigatório. Somente leitura.| 
|displayName|Cadeia de caracteres| Nome para exibição desta política. |  
|description|Cadeia de caracteres| Descrição desta política.|  
|blockMsolPowerShell|Booliano| Para desabilitar o uso do MSOL PowerShell, de definida essa propriedade como true. A configuração como true também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSOL PowerShell. Isso não afeta o Azure AD Connect ou o Microsoft Graph. | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultuserrolepermissions.md)| Especifica determinadas permissões personalizáveis para a função de usuário padrão. | 
|allowedToUseSSPR|Booliano| Indica se o Self-Serve redefinição de senha pode ser usado pelos usuários no locatário. | 
|allowedToSignUpEmailBasedSubscriptions|Booliano| Indica se os usuários podem se inscrever para assinaturas baseadas em email. | 
|allowEmailVerifiedUsersToJoinOrganization|Booliano| Indica se um usuário pode ingressar no locatário por meio de validação de email. | 
|allowInvitesFrom|Cadeia de caracteres|Indica quem pode convidar usuários externos para a organização. Os valores possíveis são:<ul><li>`none` - Impedir que todos, incluindo administradores, convidando usuários externos. Configuração padrão para o Governo dos Estados Unidos.</li><li>`adminsAndGuestInviters` - Permitir que os membros das funções Administradores Globais, Administradores de Usuários e Convidados convidem usuários externos.</li><li>`adminsGuestInvitersAndAllMembers` - Permitir que as funções de administrador acima e todos os outros membros da função de usuário convidem usuários externos.</li><li>`everyone` - Permitir que todos na organização, incluindo usuários convidados, convidem usuários externos. Configuração padrão para todos os ambientes de nuvem, exceto o Governo dos Estados Unidos.</li></ul> |

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
  "blockMsolPowerShell": true,
  "defaultUserRolePermissions": {"@odata.type": "microsoft.graph.defaultUserRolePermissions"},
  "allowedToUseSSPR": true,
  "allowedToSignUpEmailBasedSubscriptions": true,
  "allowEmailVerifiedUsersToJoinOrganization": true,
  "allowInvitesFrom": "String"
}
```

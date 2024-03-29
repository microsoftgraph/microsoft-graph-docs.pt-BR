---
title: Tipo de recurso authorizationPolicy
description: Representa uma política que pode controlar as configurações de autorização de Azure Active Directory.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 48c850a45c90f6e58e58254cbed57e30a31eac99
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854355"
---
# <a name="authorizationpolicy-resource-type"></a>Tipo de recurso authorizationPolicy

Namespace: microsoft.graph

Representa uma política que pode controlar as Azure Active Directory de autorização. É um singleton que herda do tipo de política base e sempre existe para o locatário.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter authorizationPolicy](../api/authorizationpolicy-get.md) | [authorizationPolicy](authorizationpolicy.md) | Leia o objeto authorizationPolicy. |
| [Atualizar authorizationPolicy](../api/authorizationpolicy-update.md) | Nenhum | Atualize o objeto authorizationPolicy. |

## <a name="properties"></a>Propriedades  
| Propriedade | Tipo | Descrição | 
|-|-|-|
|allowedToSignUpEmailBasedSubscriptions|Booliano| Indica se os usuários podem se inscrever para assinaturas baseadas em email. | 
|allowedToUseSSPR|Booliano| Indica se o recurso Self-Serve redefinição de senha pode ser usado pelos usuários no locatário. | 
|allowEmailVerifiedUsersToJoinOrganization|Booliano| Indica se um usuário pode ingressar no locatário por validação de email. | 
|allowInvitesFrom|allowInvitesFrom|Indica quem pode convidar usuários externos para a organização. Os valores possíveis são: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.  `everyone` é a configuração padrão para todos os ambientes de nuvem, exceto o Governo dos EUA. Confira mais na [tabela abaixo](#allowinvitesfrom-values). |
|blockMsolPowerShell|Booliano| Para desabilitar o uso do MSOL PowerShell, de definir essa propriedade como `true`. Isso também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSOL PowerShell. Isso não afeta o Azure AD Conexão ou o Microsoft Graph. | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultuserrolepermissions.md)| Especifica determinadas permissões personalizáveis para a função de usuário padrão. | 
|description|Cadeia de caracteres| Descrição dessa política.|
|displayName|String| Nome de exibição para esta política. |    
|guestUserRoleId|GUID| Representa modelo de funçãoId para a função que deve ser concedida ao usuário convidado. Atualmente, há suporte para funções a seguir: Usuário (`a0b1b346-4d3e-4e8b-98f8-753987be4970`), Usuário Convidado (`10dae51f-b6af-4016-8d66-8c2a99b929b3`) e Usuário Convidado Restrito (`2af84b1e-32c8-42b7-82bc-daa82404023b`). |
|id|String| ID da política de autorização. Obrigatório. Somente leitura.| 

### <a name="allowinvitesfrom-values"></a>valores allowInvitesFrom

|Member|Descrição|
|:---|:---|
|none|Impedir que todos, incluindo administradores, convidam usuários externos. Configuração padrão para o Governo dos EUA.|
|adminsAndGuestInviters|Permitir que os membros das funções Administradores Globais, Administradores de Usuários e Convidados convidem usuários externos.|
|adminsGuestInvitersAndAllMembers|Permitir que as funções de administrador acima e todos os outros membros da função de usuário convidem usuários externos.|
|everyone|Permitir que todos na organização, incluindo usuários convidados, convidem usuários externos. A configuração padrão para todos os ambientes de nuvem, exceto o Governo dos EUA.|

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
  "allowInvitesFrom": "String",
  "guestUserRoleId": "GUID"
}
```

---
title: tipo de recurso credentialUserRegistrationsSummary
description: Representa um resumo dos registros Azure Active Directory de credenciais de um determinado locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 43a3f5cd39e8c151c71f976042e9bb33ae527dc4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401942"
---
# <a name="credentialuserregistrationssummary-resource-type"></a>tipo de recurso credentialUserRegistrationsSummary

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um resumo dos registros Azure Active Directory de credenciais de um determinado locatário gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar credentialUserRegistrationsSummaries](../api/managedtenants-managedtenant-list-credentialuserregistrationssummaries.md)|[coleção microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md)|Obter uma lista dos [objetos credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) e suas propriedades.|
|[Obter credentialUserRegistrationsSummary](../api/managedtenants-credentialuserregistrationssummary-get.md)|[microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md)|Leia as propriedades e as relações de [um objeto credentialUserRegistrationsSummary.](../resources/managedtenants-credentialuserregistrationssummary.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo dessa entidade. Obrigatório. Somente leitura.|
|lastRefreshedDateTime|DateTimeOffset|Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento de vários locatários. Opcional. Somente leitura.|
|mfaAndSsprCapableUserCount|Int32|O número de usuários que são capazes de executar autenticação multifa factor ou redefinição de senha de autoatendados. Opcional. Somente leitura.|
|mfaConditionalAccessPolicyState|Cadeia de caracteres|O estado de uma política de acesso condicional que impõe a autenticação multifacional. Opcional. Somente leitura.|
|mfaRegisteredUserCount|Int32|O número de usuários registrados para autenticação multifa factor. Opcional. Somente leitura.|
|securityDefaultsEnabled|Boolean|Um sinalizador que indica se os Padrões de Segurança de Identidade estão habilitados. Opcional. Somente leitura.|
|ssprEnabledUserCount|Int32|O número de usuários habilitados para redefinição de senha de autoatendados. Opcional. Somente leitura.|
|ssprRegisteredUserCount|Int32|O número de usuários registrados para redefinição de senha de autoatendados. Opcional. Somente leitura.|
|tenantDisplayName|Cadeia de caracteres|O nome de exibição do locatário gerenciado. Obrigatório. Somente leitura.|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md) Obrigatório. Somente leitura.|
|totalUserCount|Int32|O número total de usuários no locatário gerenciado determinado. Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.credentialUserRegistrationsSummary",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.credentialUserRegistrationsSummary",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "mfaAndSsprCapableUserCount": "Integer",
  "ssprEnabledUserCount": "Integer",
  "mfaRegisteredUserCount": "Integer",
  "ssprRegisteredUserCount": "Integer",
  "totalUserCount": "Integer",
  "securityDefaultsEnabled": "Boolean",
  "mfaConditionalAccessPolicyState": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```

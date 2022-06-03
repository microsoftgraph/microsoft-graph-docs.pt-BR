---
title: Tipo de recurso credentialUserRegistrationsSummary
description: Representa um resumo dos registros de usuário de credencial do Azure Active Directory para um determinado locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 587925f16ab66cb6870102078ad2f885731c4832
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883856"
---
# <a name="credentialuserregistrationssummary-resource-type"></a>Tipo de recurso credentialUserRegistrationsSummary

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um resumo dos registros de usuário de credencial do Azure Active Directory para um determinado locatário gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar credentialUserRegistrationsSummaries](../api/managedtenants-managedtenant-list-credentialuserregistrationssummaries.md)|[coleção microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md)|Obtenha uma lista dos [objetos credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) e suas propriedades.|
|[Obter credentialUserRegistrationsSummary](../api/managedtenants-credentialuserregistrationssummary-get.md)|[microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md)|Leia as propriedades e as relações de um [objeto credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo dessa entidade. Obrigatório. Somente leitura.|
|lastRefreshedDateTime|DateTimeOffset|Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento multilocatário. Opcional. Somente leitura.|
|mfaAndSsprCapableUserCount|Int32|O número de usuários que são capazes de executar a autenticação multifator ou a redefinição de senha de autoatendimento. Opcional. Somente leitura.|
|mfaConditionalAccessPolicyState|String|O estado de uma política de acesso condicional que impõe a autenticação multifator. Opcional. Somente leitura.|
|mfaExcludedUserCount|Int32|O número de usuários no grupo de segurança de exclusão de autenticação multifator (exclusões do Microsoft 365 Lighthouse – MFA). Opcional. Somente leitura.|
|mfaRegisteredUserCount|Int32|O número de usuários registrados para autenticação multifator. Opcional. Somente leitura.|
|securityDefaultsEnabled|Booliano|Um sinalizador que indica se os padrões de segurança de identidade estão habilitados. Opcional. Somente leitura.|
|ssprEnabledUserCount|Int32|O número de usuários habilitados para redefinição de senha de autoatendimento. Opcional. Somente leitura.|
|ssprRegisteredUserCount|Int32|O número de usuários registrados para redefinição de senha de autoatendimento. Opcional. Somente leitura.|
|tenantDisplayName|String|O nome de exibição do locatário gerenciado. Obrigatório. Somente leitura.|
|tenantId|String|O identificador de locatário do Azure Active Directory para o [locatário gerenciado](../resources/managedtenants-tenant.md). Obrigatório. Somente leitura.|
|totalUserCount|Int32|O número total de usuários no locatário gerenciado fornecido. Opcional. Somente leitura.|

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
  "mfaExcludedUserCount": "Integer",
  "ssprEnabledUserCount": "Integer",
  "mfaRegisteredUserCount": "Integer",
  "ssprRegisteredUserCount": "Integer",
  "totalUserCount": "Integer",
  "securityDefaultsEnabled": "Boolean",
  "mfaConditionalAccessPolicyState": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```

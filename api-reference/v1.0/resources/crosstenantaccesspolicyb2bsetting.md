---
title: Tipo de recurso crossTenantAccessPolicyB2BSetting
description: Define os conjuntos de regras de entrada e saída para colaboração B2B do Azure Active Directory (Azure AD).
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: aa1740e9cde55faa8cac28c270381c3a0eff1739
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604556"
---
# <a name="crosstenantaccesspolicyb2bsetting-resource-type"></a>Tipo de recurso crossTenantAccessPolicyB2BSetting

Namespace: microsoft.graph

Define os conjuntos de regras de entrada e saída para colaboração B2B do Azure Active Directory (Azure AD).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Aplicativos|[crossTenantAccessPolicyTargetConfiguration](../resources/crosstenantaccesspolicytargetconfiguration.md)|A lista de aplicativos direcionados com sua política de acesso entre locatários.|
|usersAndGroups|[crossTenantAccessPolicyTargetConfiguration](../resources/crosstenantaccesspolicytargetconfiguration.md)|A lista de usuários e grupos direcionados com sua política de acesso entre locatários.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyB2BSetting",
  "usersAndGroups": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyTargetConfiguration"
  },
  "applications": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyTargetConfiguration"
  }
}
```

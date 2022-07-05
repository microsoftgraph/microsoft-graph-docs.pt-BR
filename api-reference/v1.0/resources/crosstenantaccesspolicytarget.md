---
title: Tipo de recurso crossTenantAccessPolicyTarget
description: Define como direcionar suas configurações de política de acesso entre locatários. As configurações podem ser direcionadas a usuários, grupos ou aplicativos específicos.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 19f58264312d8f1b519d9de9b6f66365c29f0def
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604552"
---
# <a name="crosstenantaccesspolicytarget-resource-type"></a>Tipo de recurso crossTenantAccessPolicyTarget

Namespace: microsoft.graph

Define como direcionar suas configurações de política de acesso entre locatários. As configurações podem ser direcionadas a usuários, grupos ou aplicativos específicos. Você também pode usar palavras-chave para direcionar grupos ou aplicativos específicos.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| destino | Cadeia de Caracteres | O identificador exclusivo do usuário, grupo ou aplicativo; uma das seguintes palavras-chave: `AllUsers` e `AllApplications`; ou para destinos que são aplicativos, você pode usar [valores reservados](#reserved-values-for-targets-that-are-applications). |
| Targettype | crossTenantAccessPolicyTargetType | O tipo de recurso que você deseja direcionar. Os valores possíveis são: `user`, `group`, `application`, `unknownFutureValue`. |

### <a name="reserved-values-for-targets-that-are-applications"></a>Valores reservados para destinos que são aplicativos

Ao definir destinos de aplicativo, você também pode usar os seguintes valores reservados:

| Símbolo | Descrição |
|:---|:---|
| AllMicrosoftApps | Refere-se a qualquer [aplicativo de nuvem da Microsoft](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps#microsoft-cloud-applications). |
| Office365 | Inclui os aplicativos mencionados como parte do [pacote do Office365](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps#office-365) . |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyTarget"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyTarget",
  "target": "String",
  "targetType": "microsoft.graph.crossTenantAccessPolicyTargetType"
}
```

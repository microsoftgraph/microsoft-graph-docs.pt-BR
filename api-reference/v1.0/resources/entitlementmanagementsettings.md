---
title: Tipo de recurso entitlementManagementSettings
description: Representa as configurações de todo o locatário para o gerenciamento de direitos do Azure AD.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d3b2e92db3119b302e280dd0f209af2e93a693c1
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242172"
---
# <a name="entitlementmanagementsettings-resource-type"></a>Tipo de recurso entitlementManagementSettings

Namespace: microsoft.graph


Representa configurações que controlam o comportamento do gerenciamento de direitos do [Azure AD.](entitlementmanagement-root.md)  Esse recurso não inclui a configuração de criadores de catálogos; para exibir ou alterar a associação de função de criadores de catálogo, use a [API](unifiedroleassignment.md) de atribuições de função com o provedor RBAC de gerenciamento de direitos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter direitosManagementSettings](../api/entitlementmanagementsettings-get.md)|[entitlementManagementSettings](entitlementmanagementsettings.md)|Leia as propriedades de **um objeto entitlementManagementSettings.** |
|[Update entitlementManagementSettings](../api/entitlementmanagementsettings-update.md)|[entitlementManagementSettings](entitlementmanagementsettings.md)|Atualize as propriedades de **um objeto entitlementManagementSettings.** |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|durationUntilExternalUserDeletedAfterBlocked|Duração|Se **externalUserLifecycleAction** for , a duração, normalmente um número de dias, depois que um usuário externo for bloqueado de entrar antes de sua conta `blockSignInAndDelete` ser excluída.|
|externalUserLifecycleAction|accessPackageExternalUserLifecycleAction|Ação automática que o serviço deve tomar quando a última atribuição de pacote de acesso de um usuário externo for removida. Os valores possíveis são: `none`, `blockSignIn`, `blockSignInAndDelete`, `unknownFutureValue`.|
|id|Cadeia de caracteres|Uma constante. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.entitlementManagementSettings",
  "id": "String",
  "externalUserLifecycleAction": "String",
  "durationUntilExternalUserDeletedAfterBlocked": "String (duration)"
}
```


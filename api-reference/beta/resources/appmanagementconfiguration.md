---
title: Tipo de recurso appManagementConfiguration
description: Objeto de configuração de gerenciamento de aplicativos que contém propriedades que podem ser configuradas para habilitar várias restrições para aplicativos e entidades de serviço.
author: madansr7
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c87918a001e5ede8a521f7ff666f902ba9d28b54
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695493"
---
# <a name="appmanagementconfiguration-resource-type"></a>Tipo de recurso appManagementConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Objeto de configuração de gerenciamento de aplicativos que contém propriedades que podem ser configuradas para habilitar várias restrições para aplicativos e entidades de serviço.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                                                                  | Descrição                                                                                       |
| :------------------ | :-------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------ |
| passwordCredentials | [Coleção passwordCredentialConfiguration](passwordCredentialConfiguration.md) | Conjunto de configurações de restrições de senha a serem aplicadas a um aplicativo ou entidade de serviço. |
| keyCredentials | [Coleção keyCredentialConfiguration](keyCredentialConfiguration.md) | Coleção de configurações de restrições keyCredential a serem aplicadas a um aplicativo ou entidade de serviço. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appManagementConfiguration"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.appManagementConfiguration",
  "passwordCredentials": [
    {
      "@odata.type": "microsoft.graph.passwordCredentialConfiguration"
    }
   ],
   "keyCredentials": [
    {
      "@odata.type": "microsoft.graph.keyCredentialConfiguration"
    }
   ]
}
```

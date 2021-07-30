---
title: Tipo de recurso appManagementConfiguration
description: Objeto de configuração de gerenciamento de aplicativos que contém propriedades que podem ser configuradas para habilitar várias restrições para aplicativos e entidades de serviço.
author: madansr7
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: fb8d64a746b9863116f9149a435afe9ac3998c7c
ms.sourcegitcommit: b711aed8acc18512cf6591f4108ed5ddf05b649d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2021
ms.locfileid: "53660344"
---
# <a name="appmanagementconfiguration-resource-type"></a>Tipo de recurso appManagementConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Objeto de configuração de gerenciamento de aplicativos que contém propriedades que podem ser configuradas para habilitar várias restrições para aplicativos e entidades de serviço.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                                                                  | Descrição                                                                                       |
| :------------------ | :-------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------ |
| passwordCredentials | [Coleção passwordCredentialConfiguration](passwordCredentialConfiguration.md) | Conjunto de configurações de restrições de senha a serem aplicadas a um aplicativo ou entidade de serviço |

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
   ]
}
```

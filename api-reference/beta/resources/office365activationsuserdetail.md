---
title: tipo de recurso de office365ActivationsUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a3561768e36fc63c779e19a9aa05863dd9af9315
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576882"
---
# <a name="office365activationsuserdetail-resource-type"></a>tipo de recurso de office365ActivationsUserDetail

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                     | Descrição                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| reportRefreshDate    | Data                                     | A última data do conteúdo.          |
| userPrincipalName    | String                                   | O usuário nome principal (UPN) do usuário. O UPN é um nome de logon estilo Internet para o usuário com base na Internet padrão RFC 822. Por convenção, isso deve ser mapeada para o nome de email do usuário. O formato geral é alias@domain, onde o domínio deve estar presente na coleção de locatário de domínios verificados. Essa propriedade é obrigatória quando um usuário é criado. |
| displayName          | String                                   | O nome exibido para o usuário no catálogo de endereços. Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. |
| userActivationCounts | coleção [userActivationCounts](../resources/useractivationcounts.md) | Ativação do produto mais recente do usuário a contagem de todas as plataformas para todos os tipos de produto atribuído. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userActivationCounts": [{"@odata.type":"microsoft.graph.userActivationCounts"}]
}
```

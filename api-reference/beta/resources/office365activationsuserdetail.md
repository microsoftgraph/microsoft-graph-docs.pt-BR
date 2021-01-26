---
title: Tipo de recurso office365ActivationsUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: f1bb61fa4b740c212918ee8e4794ce79ffabafe7
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980742"
---
# <a name="office365activationsuserdetail-resource-type"></a>Tipo de recurso office365ActivationsUserDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                     | Descrição                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| reportRefreshDate    | Data                                     | A data mais recente do conteúdo.          |
| userPrincipalName    | String                                   | O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. |
| displayName          | String                                   | O nome exibido para o usuário no catálogo de endereços. Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. |
| userActivationCounts | [Coleção userActivationCounts](../resources/useractivationcounts.md) | A ativação mais recente do produto do usuário conta em todas as plataformas para todos os tipos de produtos atribuídos. |

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



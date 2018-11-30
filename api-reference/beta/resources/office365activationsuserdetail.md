---
title: tipo de recurso de office365ActivationsUserDetail
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 9cf0f7f841584654176c0069fb0403a86615bfd5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035314"
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

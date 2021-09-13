---
title: Tipo de recurso office365ActivationsUserDetail
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: c70d67519ed43c36fa4bcc4df1a8d18566d732fd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057121"
---
# <a name="office365activationsuserdetail-resource-type"></a>Tipo de recurso office365ActivationsUserDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                     | Descrição                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| reportRefreshDate    | Data                                     | A data mais recente do conteúdo.          |
| userPrincipalName    | String                                   | O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. |
| displayName          | String                                   | O nome exibido para o usuário no catálogo de endereços. Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. |
| userActivationCounts | [Coleção userActivationCounts](../resources/useractivationcounts.md) | A ativação do produto mais recente do usuário conta com todas as plataformas para todos os tipos de produto atribuídos. |

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



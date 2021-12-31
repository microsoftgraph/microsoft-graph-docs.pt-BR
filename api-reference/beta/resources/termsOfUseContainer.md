---
title: Tipo de recurso termsOfUseContainer
description: Contêiner para as relações que expõem os termos de uso da API e seus recursos. Atualmente expõe os contratos e os relacionamentos agreementAcceptances.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: bef1033ceea7056d52586054f4ba32f98953cbe0
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651664"
---
# <a name="termsofusecontainer-resource-type"></a>Tipo de recurso termsOfUseContainer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner para as relações que expõem os termos de uso da API e seus recursos. Atualmente expõe os contratos [e](agreement.md) os [relacionamentos agreementAcceptances.](agreementacceptance.md)

Herda da [entidade](entity.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|agreementAcceptances|Coleção [agreementAcceptance](agreementacceptance.md)| Representa o status atual da resposta de um usuário aos termos de uso personalizáveis de uma empresa.|
|agreements|[coleção agreement](agreement.md)|Representa os termos de uso personalizáveis de um locatário que são criados e gerenciados com Azure Active Directory (Azure AD).|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsOfUseContainer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsOfUseContainer"
}
```


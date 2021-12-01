---
title: tipo complexo externalSponsors
description: Identifica uma relação com outro usuário no locatário que será permitido como aprovador.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 34db10f8efe76d324d2b6577a0e7a5efcb311dc8
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242153"
---
# <a name="externalsponsors-complex-type"></a>tipo complexo externalSponsors

Namespace: microsoft.graph

Usado no estágio de aprovação de uma política de atribuição de pacote de acesso.
É um subtipo de [subjectSet](subjectset.md), no qual o valor indica que os patrocinadores externos de uma organização conectada do usuário solicitante devem `@odata.type` ser o `#microsoft.graph.externalSponsors` aprovador. Esse aprovador só se aplica a solicitações de usuários que fazem parte de uma organização conectada.  Ao criar um estágio de aprovação da política de atribuição de pacote de acesso com externalSponsors, inclua também outro aprovador, como um único usuário ou membro do grupo, caso a organização conectada não tenha um patrocinador externo.

## <a name="properties"></a>Propriedades

Nenhum.
## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalSponsors",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalSponsors"
}
```




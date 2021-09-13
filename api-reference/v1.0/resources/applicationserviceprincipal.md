---
title: Tipo de recurso applicationServicePrincipal
description: Uma combinação de um aplicativo e um servicePrincipal.
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 3c5bafde4452842494f7890b8492b29e42bc8730
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078991"
---
# <a name="applicationserviceprincipal-resource-type"></a>Tipo de recurso applicationServicePrincipal

Namespace: microsoft.graph

Quando uma instância de um aplicativo da galeria de aplicativos do Azure AD é adicionada, os objetos [application](../resources/application.md) e [servicePrincipal](../resources/serviceprincipal.md) são criados no diretório. O **applicationServicePrincipal** representa a concatenação do **objeto** application e **servicePrincipal.**

## <a name="methods"></a>Métodos

None

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo                                                 | Descrição                                                     |
| :--------------- | :--------------------------------------------------- | :-------------------------------------------------------------- |
| application      | [aplicativo](../resources/application.md)           | Representa um aplicativo registrado no Azure Active Directory. |
| servicePrincipal | [servicePrincipal](../resources/serviceprincipal.md) | Representa uma instância de um aplicativo em um diretório.        |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationServicePrincipal",
  "keyProperty": "id"
}-->

```json
{
  "servicePrincipal": { "@odata.type": "microsoft.graph.servicePrincipal" },
  "application": { "@odata.type": "microsoft.graph.application" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

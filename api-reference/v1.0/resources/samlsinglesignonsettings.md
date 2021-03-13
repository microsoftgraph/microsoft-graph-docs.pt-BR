---
title: Tipo de recurso samlSingleSignOnSettings
description: Representa as configurações de login único SAML.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: c923c4c5b7294abb78e7fe93f852f14304601de6
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761083"
---
# <a name="samlsinglesignonsettings-resource-type"></a><span data-ttu-id="3fbf3-103">Tipo de recurso samlSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="3fbf3-103">samlSingleSignOnSettings resource type</span></span>

<span data-ttu-id="3fbf3-104">Representa um contêiner para configurações relacionadas ao login único SAML.</span><span class="sxs-lookup"><span data-stu-id="3fbf3-104">Represents a container for settings related to SAML single sign-on.</span></span>

## <a name="properties"></a><span data-ttu-id="3fbf3-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3fbf3-105">Properties</span></span>

| <span data-ttu-id="3fbf3-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fbf3-106">Property</span></span> | <span data-ttu-id="3fbf3-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fbf3-107">Type</span></span> | <span data-ttu-id="3fbf3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fbf3-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3fbf3-109">relayState</span><span class="sxs-lookup"><span data-stu-id="3fbf3-109">relayState</span></span>|<span data-ttu-id="3fbf3-110">String</span><span class="sxs-lookup"><span data-stu-id="3fbf3-110">String</span></span>| <span data-ttu-id="3fbf3-111">O URI relativo para o que o provedor de serviços redirecionaria após a conclusão do fluxo de logom único.</span><span class="sxs-lookup"><span data-stu-id="3fbf3-111">The relative URI the service provider would redirect to after completion of the single sign-on flow.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="3fbf3-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3fbf3-112">JSON representation</span></span>
<span data-ttu-id="3fbf3-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3fbf3-113">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.samlSingleSignOnSettings"
}-->

```json
{
    "relayState": "string",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "samlSingleSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

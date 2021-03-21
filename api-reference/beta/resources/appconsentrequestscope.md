---
title: Tipo de recurso appConsentRequestScope
description: Detalhes dos escopos de permissão dinâmicos para os quais o acesso é solicitado.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b960820e0d7cf20a37850256bb96ba3abf034038
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965036"
---
# <a name="appconsentrequestscope-resource-type"></a><span data-ttu-id="656e6-103">Tipo de recurso appConsentRequestScope</span><span class="sxs-lookup"><span data-stu-id="656e6-103">appConsentRequestScope resource type</span></span>

<span data-ttu-id="656e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="656e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="656e6-105">O **appConsentRequestScope** detalha os escopos de permissão dinâmicos para os quais o acesso está sendo solicitado.</span><span class="sxs-lookup"><span data-stu-id="656e6-105">The **appConsentRequestScope** details the dynamic permission scopes for which access is being requested.</span></span>

## <a name="properties"></a><span data-ttu-id="656e6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="656e6-106">Properties</span></span>
|<span data-ttu-id="656e6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="656e6-107">Property</span></span>|<span data-ttu-id="656e6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="656e6-108">Type</span></span>|<span data-ttu-id="656e6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="656e6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="656e6-110">displayName</span><span class="sxs-lookup"><span data-stu-id="656e6-110">displayName</span></span>|<span data-ttu-id="656e6-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="656e6-111">String</span></span>|<span data-ttu-id="656e6-112">O nome do escopo.</span><span class="sxs-lookup"><span data-stu-id="656e6-112">The name of the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="656e6-113">Relações</span><span class="sxs-lookup"><span data-stu-id="656e6-113">Relationships</span></span>
<span data-ttu-id="656e6-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="656e6-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="656e6-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="656e6-115">JSON representation</span></span>
<span data-ttu-id="656e6-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="656e6-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConsentRequestScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConsentRequestScope",
  "displayName": "String"
}
```


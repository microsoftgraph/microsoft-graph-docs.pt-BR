---
title: authenticationMethodConfigurations
description: objeto authenticationMethodConfigurations.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 691184b1dfbf0323204debd70488d232d77b4f7a
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761132"
---
# <a name="authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="b39d1-103">tipo de recurso authenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="b39d1-103">authenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="b39d1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b39d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b39d1-105">Representa uma política de método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b39d1-105">Represents an authentication method policy.</span></span>

## <a name="properties"></a><span data-ttu-id="b39d1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b39d1-106">Properties</span></span>
|<span data-ttu-id="b39d1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b39d1-107">Property</span></span>|<span data-ttu-id="b39d1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b39d1-108">Type</span></span>|<span data-ttu-id="b39d1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b39d1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b39d1-110">id</span><span class="sxs-lookup"><span data-stu-id="b39d1-110">id</span></span>|<span data-ttu-id="b39d1-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b39d1-111">String</span></span>|<span data-ttu-id="b39d1-112">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="b39d1-112">The policy name.</span></span>|
|<span data-ttu-id="b39d1-113">state</span><span class="sxs-lookup"><span data-stu-id="b39d1-113">state</span></span>|<span data-ttu-id="b39d1-114">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="b39d1-114">authenticationMethodState</span></span>|<span data-ttu-id="b39d1-115">O estado da política.</span><span class="sxs-lookup"><span data-stu-id="b39d1-115">The state of the policy.</span></span> <span data-ttu-id="b39d1-116">Os valores possíveis são: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="b39d1-116">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b39d1-117">Relações</span><span class="sxs-lookup"><span data-stu-id="b39d1-117">Relationships</span></span>
<span data-ttu-id="b39d1-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b39d1-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b39d1-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b39d1-119">JSON representation</span></span>
<span data-ttu-id="b39d1-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b39d1-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```

---
title: authenticationMethodConfigurations
description: objeto authenticationMethodConfigurations.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 26d0cd948a69968a7d45b3406b3da7109ffc3f18
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469126"
---
# <a name="authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="cade3-103">tipo de recurso authenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="cade3-103">authenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="cade3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cade3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cade3-105">Representa uma política de método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="cade3-105">Represents an authentication method policy.</span></span>

## <a name="properties"></a><span data-ttu-id="cade3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cade3-106">Properties</span></span>
|<span data-ttu-id="cade3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cade3-107">Property</span></span>|<span data-ttu-id="cade3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cade3-108">Type</span></span>|<span data-ttu-id="cade3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cade3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cade3-110">id</span><span class="sxs-lookup"><span data-stu-id="cade3-110">id</span></span>|<span data-ttu-id="cade3-111">String</span><span class="sxs-lookup"><span data-stu-id="cade3-111">String</span></span>|<span data-ttu-id="cade3-112">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="cade3-112">The policy name.</span></span>|
|<span data-ttu-id="cade3-113">state</span><span class="sxs-lookup"><span data-stu-id="cade3-113">state</span></span>|<span data-ttu-id="cade3-114">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="cade3-114">authenticationMethodState</span></span>|<span data-ttu-id="cade3-115">O estado da política.</span><span class="sxs-lookup"><span data-stu-id="cade3-115">The state of the policy.</span></span> <span data-ttu-id="cade3-116">Os valores possíveis são: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="cade3-116">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cade3-117">Relações</span><span class="sxs-lookup"><span data-stu-id="cade3-117">Relationships</span></span>
<span data-ttu-id="cade3-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cade3-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cade3-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cade3-119">JSON representation</span></span>
<span data-ttu-id="cade3-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cade3-120">The following is a JSON representation of the resource.</span></span>
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

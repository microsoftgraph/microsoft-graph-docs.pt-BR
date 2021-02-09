---
title: authenticationMethodConfigurations
description: Objeto authenticationMethodConfigurations.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cda2cda7756bb795c93e10dddbd344e5a4a92ed2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159133"
---
# <a name="authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="35506-103">Tipo de recurso authenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="35506-103">authenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="35506-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35506-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35506-105">Representa uma política de método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="35506-105">Represents an authentication method policy.</span></span>

## <a name="properties"></a><span data-ttu-id="35506-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35506-106">Properties</span></span>
|<span data-ttu-id="35506-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35506-107">Property</span></span>|<span data-ttu-id="35506-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="35506-108">Type</span></span>|<span data-ttu-id="35506-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="35506-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35506-110">id</span><span class="sxs-lookup"><span data-stu-id="35506-110">id</span></span>|<span data-ttu-id="35506-111">String</span><span class="sxs-lookup"><span data-stu-id="35506-111">String</span></span>|<span data-ttu-id="35506-112">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="35506-112">The policy name.</span></span>|
|<span data-ttu-id="35506-113">estado</span><span class="sxs-lookup"><span data-stu-id="35506-113">state</span></span>|<span data-ttu-id="35506-114">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="35506-114">authenticationMethodState</span></span>|<span data-ttu-id="35506-115">O estado da política.</span><span class="sxs-lookup"><span data-stu-id="35506-115">The state of the policy.</span></span> <span data-ttu-id="35506-116">Os valores possíveis são: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="35506-116">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35506-117">Relações</span><span class="sxs-lookup"><span data-stu-id="35506-117">Relationships</span></span>
<span data-ttu-id="35506-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35506-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="35506-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35506-119">JSON representation</span></span>
<span data-ttu-id="35506-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35506-120">The following is a JSON representation of the resource.</span></span>
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

---
title: Tipo de recurso servicePrincipalIdentity
description: Modela uma identidade de entidade de serviço.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a49adab87ac5ebe7b8eddf106d8d38c4e15acd11
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469723"
---
# <a name="serviceprincipalidentity-resource-type"></a><span data-ttu-id="71f70-103">Tipo de recurso servicePrincipalIdentity</span><span class="sxs-lookup"><span data-stu-id="71f70-103">servicePrincipalIdentity resource type</span></span>

<span data-ttu-id="71f70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71f70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71f70-105">Modela uma identidade de entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="71f70-105">Models a service principal identity.</span></span>

<span data-ttu-id="71f70-106">Herda da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="71f70-106">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="71f70-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71f70-107">Properties</span></span>
|<span data-ttu-id="71f70-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71f70-108">Property</span></span>|<span data-ttu-id="71f70-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="71f70-109">Type</span></span>|<span data-ttu-id="71f70-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="71f70-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71f70-111">appId</span><span class="sxs-lookup"><span data-stu-id="71f70-111">appId</span></span>|<span data-ttu-id="71f70-112">String</span><span class="sxs-lookup"><span data-stu-id="71f70-112">String</span></span>| <span data-ttu-id="71f70-113">O identificador de aplicativo da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="71f70-113">The application identifier of the service principal.</span></span> |
|<span data-ttu-id="71f70-114">displayName</span><span class="sxs-lookup"><span data-stu-id="71f70-114">displayName</span></span>|<span data-ttu-id="71f70-115">String</span><span class="sxs-lookup"><span data-stu-id="71f70-115">String</span></span>| <span data-ttu-id="71f70-116">O nome de exibição da identidade da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="71f70-116">The display name of the service principal identity.</span></span> <span data-ttu-id="71f70-117">Herdado da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="71f70-117">Inherited from [identity](../resources/identity.md).</span></span> |
|<span data-ttu-id="71f70-118">id</span><span class="sxs-lookup"><span data-stu-id="71f70-118">id</span></span>|<span data-ttu-id="71f70-119">String</span><span class="sxs-lookup"><span data-stu-id="71f70-119">String</span></span>| <span data-ttu-id="71f70-120">O identificador da identidade da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="71f70-120">The identifier of the service principal identity.</span></span> <span data-ttu-id="71f70-121">Herdado da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="71f70-121">Inherited from [identity](../resources/identity.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="71f70-122">Relações</span><span class="sxs-lookup"><span data-stu-id="71f70-122">Relationships</span></span>
<span data-ttu-id="71f70-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71f70-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="71f70-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71f70-124">JSON representation</span></span>
<span data-ttu-id="71f70-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71f70-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.servicePrincipalIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.servicePrincipalIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "appId": "String"
}
```

---
title: Tipo de recurso servicePrincipalIdentity
description: Modela uma identidade de entidade de serviço.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 231a0d9dc811569de23412d6ad76a2ba35f6c58b
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031023"
---
# <a name="serviceprincipalidentity-resource-type"></a><span data-ttu-id="d4f31-103">Tipo de recurso servicePrincipalIdentity</span><span class="sxs-lookup"><span data-stu-id="d4f31-103">servicePrincipalIdentity resource type</span></span>

<span data-ttu-id="d4f31-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4f31-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4f31-105">Modela uma identidade de entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="d4f31-105">Models a service principal identity.</span></span>

<span data-ttu-id="d4f31-106">Herda da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="d4f31-106">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d4f31-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4f31-107">Properties</span></span>
|<span data-ttu-id="d4f31-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4f31-108">Property</span></span>|<span data-ttu-id="d4f31-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4f31-109">Type</span></span>|<span data-ttu-id="d4f31-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4f31-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4f31-111">appId</span><span class="sxs-lookup"><span data-stu-id="d4f31-111">appId</span></span>|<span data-ttu-id="d4f31-112">String</span><span class="sxs-lookup"><span data-stu-id="d4f31-112">String</span></span>|<span data-ttu-id="d4f31-113">O identificador de aplicativo da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="d4f31-113">The application identifier of the service principal.</span></span>|
|<span data-ttu-id="d4f31-114">displayName</span><span class="sxs-lookup"><span data-stu-id="d4f31-114">displayName</span></span>|<span data-ttu-id="d4f31-115">String</span><span class="sxs-lookup"><span data-stu-id="d4f31-115">String</span></span>|<span data-ttu-id="d4f31-116">O nome de exibição da identidade da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="d4f31-116">The display name of the service principal identity.</span></span> <span data-ttu-id="d4f31-117">Herdado da [identidade](../resources/identity.md)</span><span class="sxs-lookup"><span data-stu-id="d4f31-117">Inherited from [identity](../resources/identity.md)</span></span>|
|<span data-ttu-id="d4f31-118">id</span><span class="sxs-lookup"><span data-stu-id="d4f31-118">id</span></span>|<span data-ttu-id="d4f31-119">String</span><span class="sxs-lookup"><span data-stu-id="d4f31-119">String</span></span>|<span data-ttu-id="d4f31-120">O identificador da identidade da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="d4f31-120">The identifier of the service principal identity.</span></span> <span data-ttu-id="d4f31-121">Herdado da [identidade](../resources/identity.md)</span><span class="sxs-lookup"><span data-stu-id="d4f31-121">Inherited from [identity](../resources/identity.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4f31-122">Relações</span><span class="sxs-lookup"><span data-stu-id="d4f31-122">Relationships</span></span>
<span data-ttu-id="d4f31-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4f31-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4f31-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4f31-124">JSON representation</span></span>
<span data-ttu-id="d4f31-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4f31-125">The following is a JSON representation of the resource.</span></span>
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

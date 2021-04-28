---
title: Tipo de recurso accessReviewPolicy
description: A política de revisões do Access é um singleton que permite que as organizações gerenciem a política de revisão de acesso no nível do diretório.
author: kafen
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 02940987682d84aa3fc3dbb076c998abfe24bf8e
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067811"
---
# <a name="accessreviewpolicy-resource-type"></a><span data-ttu-id="299b3-103">Tipo de recurso accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="299b3-103">accessReviewPolicy resource type</span></span>

<span data-ttu-id="299b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="299b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="299b3-105">A política de revisão do Access é um singleton que permite que os administradores gerenciem políticas de revisão de acesso no nível do diretório.</span><span class="sxs-lookup"><span data-stu-id="299b3-105">Access review policy is a singleton that enables administrators to manage directory-level access review policies.</span></span> <span data-ttu-id="299b3-106">Por exemplo, os administradores podem usar a política de revisão de acesso para habilitar e desabilitar a capacidade dos proprietários do grupo de criar avaliações de acesso nos grupos que eles têm.</span><span class="sxs-lookup"><span data-stu-id="299b3-106">For example, administrators can use the access review policy to enable and disable the ability of group owners to create access reviews on groups that they own.</span></span>


<span data-ttu-id="299b3-107">Herda da [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="299b3-107">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="299b3-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="299b3-108">Methods</span></span>
|<span data-ttu-id="299b3-109">Método</span><span class="sxs-lookup"><span data-stu-id="299b3-109">Method</span></span>|<span data-ttu-id="299b3-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="299b3-110">Return type</span></span>|<span data-ttu-id="299b3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="299b3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="299b3-112">Obter accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="299b3-112">Get accessReviewPolicy</span></span>](../api/accessreviewpolicy-get.md)|[<span data-ttu-id="299b3-113">accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="299b3-113">accessReviewPolicy</span></span>](../resources/accessreviewpolicy.md)|<span data-ttu-id="299b3-114">Leia as propriedades e as relações de um [objeto accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="299b3-114">Read the properties and relationships of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>|
|[<span data-ttu-id="299b3-115">Atualizar accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="299b3-115">Update accessReviewPolicy</span></span>](../api/accessreviewpolicy-update.md)|[<span data-ttu-id="299b3-116">accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="299b3-116">accessReviewPolicy</span></span>](../resources/accessreviewpolicy.md)|<span data-ttu-id="299b3-117">Atualize as propriedades de [um objeto accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="299b3-117">Update the properties of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="299b3-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="299b3-118">Properties</span></span>
|<span data-ttu-id="299b3-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="299b3-119">Property</span></span>|<span data-ttu-id="299b3-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="299b3-120">Type</span></span>|<span data-ttu-id="299b3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="299b3-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="299b3-122">description</span><span class="sxs-lookup"><span data-stu-id="299b3-122">description</span></span>|<span data-ttu-id="299b3-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="299b3-123">String</span></span>|<span data-ttu-id="299b3-124">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="299b3-124">Description for this policy.</span></span> <span data-ttu-id="299b3-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="299b3-125">Read-only.</span></span>|
|<span data-ttu-id="299b3-126">displayName</span><span class="sxs-lookup"><span data-stu-id="299b3-126">displayName</span></span>|<span data-ttu-id="299b3-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="299b3-127">String</span></span>|<span data-ttu-id="299b3-128">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="299b3-128">Display name for this policy.</span></span> <span data-ttu-id="299b3-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="299b3-129">Read-only.</span></span>|
|<span data-ttu-id="299b3-130">isGroupOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="299b3-130">isGroupOwnerManagementEnabled</span></span>|<span data-ttu-id="299b3-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="299b3-131">Boolean</span></span>|<span data-ttu-id="299b3-132">Se `true` , os proprietários do grupo podem criar e gerenciar avaliações de acesso nos grupos que eles próprios têm.</span><span class="sxs-lookup"><span data-stu-id="299b3-132">If `true`, group owners can create and manage access reviews on groups they own.</span></span>|

## <a name="relationships"></a><span data-ttu-id="299b3-133">Relações</span><span class="sxs-lookup"><span data-stu-id="299b3-133">Relationships</span></span>
<span data-ttu-id="299b3-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="299b3-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="299b3-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="299b3-135">JSON representation</span></span>
<span data-ttu-id="299b3-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="299b3-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewPolicy",
  "displayName": "Access Review Policy",
  "description": "Policy contains directory-level access review settings.",
  "isGroupOwnerManagementEnabled": false
}
```

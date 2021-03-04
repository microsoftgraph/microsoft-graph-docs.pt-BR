---
title: Tipo de recurso userSource
description: O contêiner para a caixa de correio de um custodiado e o site do OneDrive for Business.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f0d98ac894d3d60bed2bb249ef9daec707f6f7ba
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445941"
---
# <a name="usersource-resource-type"></a><span data-ttu-id="3e85e-103">Tipo de recurso userSource</span><span class="sxs-lookup"><span data-stu-id="3e85e-103">userSource resource type</span></span>

<span data-ttu-id="3e85e-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="3e85e-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e85e-105">O contêiner para a [caixa de correio de um custodiado](ediscovery-custodian.md) e o site do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="3e85e-105">The container for a [custodian's](ediscovery-custodian.md) mailbox and OneDrive for Business site.</span></span>

## <a name="methods"></a><span data-ttu-id="3e85e-106">Methods</span><span class="sxs-lookup"><span data-stu-id="3e85e-106">Methods</span></span>

|<span data-ttu-id="3e85e-107">Método</span><span class="sxs-lookup"><span data-stu-id="3e85e-107">Method</span></span>|<span data-ttu-id="3e85e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3e85e-108">Return type</span></span>|<span data-ttu-id="3e85e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e85e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3e85e-110">Listar userSources</span><span class="sxs-lookup"><span data-stu-id="3e85e-110">List userSources</span></span>](../api/ediscovery-custodian-list-usersources.md)|<span data-ttu-id="3e85e-111">[coleção microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)</span><span class="sxs-lookup"><span data-stu-id="3e85e-111">[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) collection</span></span>|<span data-ttu-id="3e85e-112">Obter uma lista dos **objetos userSource** e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="3e85e-112">Get a list of the **userSource** objects and their properties.</span></span>|
|[<span data-ttu-id="3e85e-113">Criar userSource</span><span class="sxs-lookup"><span data-stu-id="3e85e-113">Create userSource</span></span>](../api/ediscovery-custodian-post-usersources.md)|[<span data-ttu-id="3e85e-114">microsoft.graph.ediscovery.userSource</span><span class="sxs-lookup"><span data-stu-id="3e85e-114">microsoft.graph.ediscovery.userSource</span></span>](../resources/ediscovery-usersource.md)|<span data-ttu-id="3e85e-115">Crie um novo **objeto userSource.**</span><span class="sxs-lookup"><span data-stu-id="3e85e-115">Create a new **userSource** object.</span></span>|
|[<span data-ttu-id="3e85e-116">Obter userSource</span><span class="sxs-lookup"><span data-stu-id="3e85e-116">Get userSource</span></span>](../api/ediscovery-usersource-get.md)|[<span data-ttu-id="3e85e-117">microsoft.graph.ediscovery.userSource</span><span class="sxs-lookup"><span data-stu-id="3e85e-117">microsoft.graph.ediscovery.userSource</span></span>](../resources/ediscovery-usersource.md)|<span data-ttu-id="3e85e-118">Leia as propriedades e as relações de um **objeto userSource.**</span><span class="sxs-lookup"><span data-stu-id="3e85e-118">Read the properties and relationships of a **userSource** object.</span></span>|
|[<span data-ttu-id="3e85e-119">Excluir userSource</span><span class="sxs-lookup"><span data-stu-id="3e85e-119">Delete userSource</span></span>](../api/ediscovery-usersource-delete.md)|<span data-ttu-id="3e85e-120">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="3e85e-120">None</span></span>|<span data-ttu-id="3e85e-121">**Exclua um objeto userSource.**</span><span class="sxs-lookup"><span data-stu-id="3e85e-121">Delete a **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3e85e-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e85e-122">Properties</span></span>

|<span data-ttu-id="3e85e-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e85e-123">Property</span></span>|<span data-ttu-id="3e85e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e85e-124">Type</span></span>|<span data-ttu-id="3e85e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e85e-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e85e-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="3e85e-126">createdBy</span></span>|[<span data-ttu-id="3e85e-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="3e85e-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="3e85e-128">O usuário que criou **o userSource**.</span><span class="sxs-lookup"><span data-stu-id="3e85e-128">The user who created the **userSource**.</span></span>|
|<span data-ttu-id="3e85e-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e85e-129">createdDateTime</span></span>|<span data-ttu-id="3e85e-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e85e-130">DateTimeOffset</span></span>|<span data-ttu-id="3e85e-131">A data e a hora **em que o userSource** foi criado</span><span class="sxs-lookup"><span data-stu-id="3e85e-131">The date and time the **userSource** was created</span></span>|
|<span data-ttu-id="3e85e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="3e85e-132">displayName</span></span>|<span data-ttu-id="3e85e-133">String</span><span class="sxs-lookup"><span data-stu-id="3e85e-133">String</span></span>|<span data-ttu-id="3e85e-134">O nome de exibição associado à caixa de correio e ao site.</span><span class="sxs-lookup"><span data-stu-id="3e85e-134">The display name associated with the mailbox and site.</span></span>|
|<span data-ttu-id="3e85e-135">email</span><span class="sxs-lookup"><span data-stu-id="3e85e-135">email</span></span>|<span data-ttu-id="3e85e-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e85e-136">String</span></span>|<span data-ttu-id="3e85e-137">Endereço de email da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="3e85e-137">Email address of the user's mailbox.</span></span>|
|<span data-ttu-id="3e85e-138">id</span><span class="sxs-lookup"><span data-stu-id="3e85e-138">id</span></span>|<span data-ttu-id="3e85e-139">String</span><span class="sxs-lookup"><span data-stu-id="3e85e-139">String</span></span>|<span data-ttu-id="3e85e-140">A ID do **userSource**.</span><span class="sxs-lookup"><span data-stu-id="3e85e-140">The ID of the **userSource**.</span></span> <span data-ttu-id="3e85e-141">Essa não é a ID do grupo real</span><span class="sxs-lookup"><span data-stu-id="3e85e-141">This is not the ID of the actual group</span></span>|
|<span data-ttu-id="3e85e-142">includedSources</span><span class="sxs-lookup"><span data-stu-id="3e85e-142">includedSources</span></span>|<span data-ttu-id="3e85e-143">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="3e85e-143">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="3e85e-144">Especifica quais fontes estão incluídas neste grupo.</span><span class="sxs-lookup"><span data-stu-id="3e85e-144">Specifies which sources are included in this group.</span></span> <span data-ttu-id="3e85e-145">Os valores possíveis são: `mailbox` e `site`.</span><span class="sxs-lookup"><span data-stu-id="3e85e-145">Possible values are: `mailbox`, `site`.</span></span>|

### <a name="sourcetype-values"></a><span data-ttu-id="3e85e-146">valores sourceType</span><span class="sxs-lookup"><span data-stu-id="3e85e-146">sourceType values</span></span>

<span data-ttu-id="3e85e-147">Tipos de fonte relacionados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="3e85e-147">Types of source related to the user.</span></span> <span data-ttu-id="3e85e-148">Inclui caixa de correio e site por padrão.</span><span class="sxs-lookup"><span data-stu-id="3e85e-148">Includes mailbox and site by default.</span></span>

|<span data-ttu-id="3e85e-149">Member</span><span class="sxs-lookup"><span data-stu-id="3e85e-149">Member</span></span>|<span data-ttu-id="3e85e-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e85e-150">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="3e85e-151">mailbox</span><span class="sxs-lookup"><span data-stu-id="3e85e-151">mailbox</span></span>|<span data-ttu-id="3e85e-152">Representa uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="3e85e-152">Represents a mailbox.</span></span>|
|<span data-ttu-id="3e85e-153">site</span><span class="sxs-lookup"><span data-stu-id="3e85e-153">site</span></span>|<span data-ttu-id="3e85e-154">Representa um site do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="3e85e-154">Represents a OneDrive for Business site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e85e-155">Relações</span><span class="sxs-lookup"><span data-stu-id="3e85e-155">Relationships</span></span>

<span data-ttu-id="3e85e-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3e85e-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e85e-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e85e-157">JSON representation</span></span>

<span data-ttu-id="3e85e-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e85e-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.userSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.userSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "email": "String",
  "includedSources": "String"
}
```

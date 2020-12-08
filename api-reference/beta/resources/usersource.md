---
title: tipo de recurso username
description: O contêiner para a caixa de correio de um dos responsáveis e o site do OneDrive for Business.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 2ce5448947bded580cc4896ba549d7cc6fab95f9
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597482"
---
# <a name="usersource-resource-type"></a><span data-ttu-id="e01f5-103">tipo de recurso username</span><span class="sxs-lookup"><span data-stu-id="e01f5-103">userSource resource type</span></span>

<span data-ttu-id="e01f5-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e01f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e01f5-105">O contêiner para a caixa de correio de um dos responsáveis e o site [do](custodian.md) onedrive for Business.</span><span class="sxs-lookup"><span data-stu-id="e01f5-105">The container for a [custodian's](custodian.md) mailbox and OneDrive for Business site.</span></span>

## <a name="methods"></a><span data-ttu-id="e01f5-106">Methods</span><span class="sxs-lookup"><span data-stu-id="e01f5-106">Methods</span></span>

|<span data-ttu-id="e01f5-107">Método</span><span class="sxs-lookup"><span data-stu-id="e01f5-107">Method</span></span>|<span data-ttu-id="e01f5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e01f5-108">Return type</span></span>|<span data-ttu-id="e01f5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e01f5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e01f5-110">Listar usersources</span><span class="sxs-lookup"><span data-stu-id="e01f5-110">List userSources</span></span>](../api/custodian-list-usersources.md)|<span data-ttu-id="e01f5-111">coleção [username](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="e01f5-111">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="e01f5-112">Obtenha uma lista dos objetos **username** e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="e01f5-112">Get a list of the **userSource** objects and their properties.</span></span>|
|[<span data-ttu-id="e01f5-113">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="e01f5-113">Create userSource</span></span>](../api/custodian-post-usersources.md)|[<span data-ttu-id="e01f5-114">username</span><span class="sxs-lookup"><span data-stu-id="e01f5-114">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="e01f5-115">Criar um novo objeto **username** .</span><span class="sxs-lookup"><span data-stu-id="e01f5-115">Create a new **userSource** object.</span></span>|
|[<span data-ttu-id="e01f5-116">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="e01f5-116">Get userSource</span></span>](../api/usersource-get.md)|[<span data-ttu-id="e01f5-117">username</span><span class="sxs-lookup"><span data-stu-id="e01f5-117">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="e01f5-118">Leia as propriedades e os relacionamentos de um objeto **username** .</span><span class="sxs-lookup"><span data-stu-id="e01f5-118">Read the properties and relationships of a **userSource** object.</span></span>|
|[<span data-ttu-id="e01f5-119">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="e01f5-119">Delete userSource</span></span>](../api/usersource-delete.md)|<span data-ttu-id="e01f5-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e01f5-120">None</span></span>|<span data-ttu-id="e01f5-121">Excluir um objeto **username** .</span><span class="sxs-lookup"><span data-stu-id="e01f5-121">Delete a **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e01f5-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e01f5-122">Properties</span></span>

|<span data-ttu-id="e01f5-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e01f5-123">Property</span></span>|<span data-ttu-id="e01f5-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="e01f5-124">Type</span></span>|<span data-ttu-id="e01f5-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e01f5-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e01f5-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="e01f5-126">createdBy</span></span>|[<span data-ttu-id="e01f5-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="e01f5-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="e01f5-128">O usuário que criou a **username**.</span><span class="sxs-lookup"><span data-stu-id="e01f5-128">The user who created the **userSource**.</span></span>|
|<span data-ttu-id="e01f5-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e01f5-129">createdDateTime</span></span>|<span data-ttu-id="e01f5-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e01f5-130">DateTimeOffset</span></span>|<span data-ttu-id="e01f5-131">A data e a hora em que o **usuário** da erSource foi criado</span><span class="sxs-lookup"><span data-stu-id="e01f5-131">The date and time the us **userSource** erSource was created</span></span>|
|<span data-ttu-id="e01f5-132">displayName</span><span class="sxs-lookup"><span data-stu-id="e01f5-132">displayName</span></span>|<span data-ttu-id="e01f5-133">String</span><span class="sxs-lookup"><span data-stu-id="e01f5-133">String</span></span>|<span data-ttu-id="e01f5-134">O nome de exibição associado à caixa de correio e ao site.</span><span class="sxs-lookup"><span data-stu-id="e01f5-134">The display name associated with the mailbox and site.</span></span>|
|<span data-ttu-id="e01f5-135">email</span><span class="sxs-lookup"><span data-stu-id="e01f5-135">email</span></span>|<span data-ttu-id="e01f5-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e01f5-136">String</span></span>|<span data-ttu-id="e01f5-137">Endereço de email da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="e01f5-137">Email address of the user's mailbox.</span></span>|
|<span data-ttu-id="e01f5-138">id</span><span class="sxs-lookup"><span data-stu-id="e01f5-138">id</span></span>|<span data-ttu-id="e01f5-139">String</span><span class="sxs-lookup"><span data-stu-id="e01f5-139">String</span></span>|<span data-ttu-id="e01f5-140">A ID da **username**.</span><span class="sxs-lookup"><span data-stu-id="e01f5-140">The ID of the **userSource**.</span></span> <span data-ttu-id="e01f5-141">Essa não é a ID do grupo real</span><span class="sxs-lookup"><span data-stu-id="e01f5-141">This is not the ID of the actual group</span></span>|
|<span data-ttu-id="e01f5-142">includedSources</span><span class="sxs-lookup"><span data-stu-id="e01f5-142">includedSources</span></span>|<span data-ttu-id="e01f5-143">sourceType</span><span class="sxs-lookup"><span data-stu-id="e01f5-143">sourceType</span></span>|<span data-ttu-id="e01f5-144">Especifica quais fontes são incluídas nesse grupo.</span><span class="sxs-lookup"><span data-stu-id="e01f5-144">Specifies which sources are included in this group.</span></span> <span data-ttu-id="e01f5-145">Os valores possíveis são: `mailbox` e `site`.</span><span class="sxs-lookup"><span data-stu-id="e01f5-145">Possible values are: `mailbox`, `site`.</span></span>|

### <a name="sourcetype-values"></a><span data-ttu-id="e01f5-146">valores de sourceType</span><span class="sxs-lookup"><span data-stu-id="e01f5-146">sourceType values</span></span>

<span data-ttu-id="e01f5-147">Tipos de fonte relacionados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="e01f5-147">Types of source related to the user.</span></span> <span data-ttu-id="e01f5-148">Inclui a caixa de correio e o site por padrão.</span><span class="sxs-lookup"><span data-stu-id="e01f5-148">Includes mailbox and site by default.</span></span>

|<span data-ttu-id="e01f5-149">Member</span><span class="sxs-lookup"><span data-stu-id="e01f5-149">Member</span></span>|<span data-ttu-id="e01f5-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="e01f5-150">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="e01f5-151">mailbox</span><span class="sxs-lookup"><span data-stu-id="e01f5-151">mailbox</span></span>|<span data-ttu-id="e01f5-152">Representa uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e01f5-152">Represents a mailbox.</span></span>|
|<span data-ttu-id="e01f5-153">site</span><span class="sxs-lookup"><span data-stu-id="e01f5-153">site</span></span>|<span data-ttu-id="e01f5-154">Representa um site do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="e01f5-154">Represents a OneDrive for Business site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e01f5-155">Relações</span><span class="sxs-lookup"><span data-stu-id="e01f5-155">Relationships</span></span>

<span data-ttu-id="e01f5-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e01f5-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e01f5-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e01f5-157">JSON representation</span></span>

<span data-ttu-id="e01f5-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e01f5-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSource",
  "baseType": "microsoft.graph.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userSource",
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

---
title: tipo de recurso username
description: O contêiner para a caixa de correio de um dos responsáveis e o site do OneDrive for Business.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 10184e053a0c62aaba6599f7d6f9bb6a33de8828
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706035"
---
# <a name="usersource-resource-type"></a><span data-ttu-id="0034f-103">tipo de recurso username</span><span class="sxs-lookup"><span data-stu-id="0034f-103">userSource resource type</span></span>

<span data-ttu-id="0034f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0034f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0034f-105">O contêiner para a caixa de correio de um dos responsáveis e o site [do](custodian.md) onedrive for Business.</span><span class="sxs-lookup"><span data-stu-id="0034f-105">The container for a [custodian's](custodian.md) mailbox and OneDrive for Business site.</span></span>

## <a name="methods"></a><span data-ttu-id="0034f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="0034f-106">Methods</span></span>

|<span data-ttu-id="0034f-107">Método</span><span class="sxs-lookup"><span data-stu-id="0034f-107">Method</span></span>|<span data-ttu-id="0034f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0034f-108">Return type</span></span>|<span data-ttu-id="0034f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0034f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0034f-110">Listar usersources</span><span class="sxs-lookup"><span data-stu-id="0034f-110">List userSources</span></span>](../api/custodian-list-usersources.md)|<span data-ttu-id="0034f-111">coleção [username](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="0034f-111">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="0034f-112">Obtenha uma lista dos objetos **username** e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="0034f-112">Get a list of the **userSource** objects and their properties.</span></span>|
|[<span data-ttu-id="0034f-113">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="0034f-113">Create userSource</span></span>](../api/custodian-post-usersources.md)|[<span data-ttu-id="0034f-114">username</span><span class="sxs-lookup"><span data-stu-id="0034f-114">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="0034f-115">Criar um novo objeto **username** .</span><span class="sxs-lookup"><span data-stu-id="0034f-115">Create a new **userSource** object.</span></span>|
|[<span data-ttu-id="0034f-116">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="0034f-116">Get userSource</span></span>](../api/usersource-get.md)|[<span data-ttu-id="0034f-117">username</span><span class="sxs-lookup"><span data-stu-id="0034f-117">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="0034f-118">Leia as propriedades e os relacionamentos de um objeto **username** .</span><span class="sxs-lookup"><span data-stu-id="0034f-118">Read the properties and relationships of a **userSource** object.</span></span>|
|[<span data-ttu-id="0034f-119">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="0034f-119">Delete userSource</span></span>](../api/usersource-delete.md)|<span data-ttu-id="0034f-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0034f-120">None</span></span>|<span data-ttu-id="0034f-121">Excluir um objeto **username** .</span><span class="sxs-lookup"><span data-stu-id="0034f-121">Delete a **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0034f-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0034f-122">Properties</span></span>

|<span data-ttu-id="0034f-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0034f-123">Property</span></span>|<span data-ttu-id="0034f-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="0034f-124">Type</span></span>|<span data-ttu-id="0034f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0034f-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0034f-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="0034f-126">createdBy</span></span>|[<span data-ttu-id="0034f-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="0034f-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="0034f-128">O usuário que criou a **username**.</span><span class="sxs-lookup"><span data-stu-id="0034f-128">The user who created the **userSource**.</span></span>|
|<span data-ttu-id="0034f-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0034f-129">createdDateTime</span></span>|<span data-ttu-id="0034f-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0034f-130">DateTimeOffset</span></span>|<span data-ttu-id="0034f-131">A data e a hora em que o **username** foi criado</span><span class="sxs-lookup"><span data-stu-id="0034f-131">The date and time the **userSource** was created</span></span>|
|<span data-ttu-id="0034f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0034f-132">displayName</span></span>|<span data-ttu-id="0034f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0034f-133">String</span></span>|<span data-ttu-id="0034f-134">O nome de exibição associado à caixa de correio e ao site.</span><span class="sxs-lookup"><span data-stu-id="0034f-134">The display name associated with the mailbox and site.</span></span>|
|<span data-ttu-id="0034f-135">email</span><span class="sxs-lookup"><span data-stu-id="0034f-135">email</span></span>|<span data-ttu-id="0034f-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0034f-136">String</span></span>|<span data-ttu-id="0034f-137">Endereço de email da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="0034f-137">Email address of the user's mailbox.</span></span>|
|<span data-ttu-id="0034f-138">id</span><span class="sxs-lookup"><span data-stu-id="0034f-138">id</span></span>|<span data-ttu-id="0034f-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0034f-139">String</span></span>|<span data-ttu-id="0034f-140">A ID da **username**.</span><span class="sxs-lookup"><span data-stu-id="0034f-140">The ID of the **userSource**.</span></span> <span data-ttu-id="0034f-141">Essa não é a ID do grupo real</span><span class="sxs-lookup"><span data-stu-id="0034f-141">This is not the ID of the actual group</span></span>|
|<span data-ttu-id="0034f-142">includedSources</span><span class="sxs-lookup"><span data-stu-id="0034f-142">includedSources</span></span>|<span data-ttu-id="0034f-143">sourceType</span><span class="sxs-lookup"><span data-stu-id="0034f-143">sourceType</span></span>|<span data-ttu-id="0034f-144">Especifica quais fontes são incluídas nesse grupo.</span><span class="sxs-lookup"><span data-stu-id="0034f-144">Specifies which sources are included in this group.</span></span> <span data-ttu-id="0034f-145">Os valores possíveis são: `mailbox` e `site`.</span><span class="sxs-lookup"><span data-stu-id="0034f-145">Possible values are: `mailbox`, `site`.</span></span>|

### <a name="sourcetype-values"></a><span data-ttu-id="0034f-146">valores de sourceType</span><span class="sxs-lookup"><span data-stu-id="0034f-146">sourceType values</span></span>

<span data-ttu-id="0034f-147">Tipos de fonte relacionados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="0034f-147">Types of source related to the user.</span></span> <span data-ttu-id="0034f-148">Inclui a caixa de correio e o site por padrão.</span><span class="sxs-lookup"><span data-stu-id="0034f-148">Includes mailbox and site by default.</span></span>

|<span data-ttu-id="0034f-149">Member</span><span class="sxs-lookup"><span data-stu-id="0034f-149">Member</span></span>|<span data-ttu-id="0034f-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="0034f-150">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="0034f-151">mailbox</span><span class="sxs-lookup"><span data-stu-id="0034f-151">mailbox</span></span>|<span data-ttu-id="0034f-152">Representa uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0034f-152">Represents a mailbox.</span></span>|
|<span data-ttu-id="0034f-153">site</span><span class="sxs-lookup"><span data-stu-id="0034f-153">site</span></span>|<span data-ttu-id="0034f-154">Representa um site do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="0034f-154">Represents a OneDrive for Business site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0034f-155">Relações</span><span class="sxs-lookup"><span data-stu-id="0034f-155">Relationships</span></span>

<span data-ttu-id="0034f-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0034f-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0034f-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0034f-157">JSON representation</span></span>

<span data-ttu-id="0034f-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0034f-158">The following is a JSON representation of the resource.</span></span>
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

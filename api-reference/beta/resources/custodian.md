---
title: tipo de recurso responsáveis
description: No contexto da descoberta eletrônica, representa um usuário e todos os seus ativos digitais, como emails e documentos.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: a2e22f711eaec4cd68cc5026e36b900d5284e71a
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597531"
---
# <a name="custodian-resource-type"></a><span data-ttu-id="81f37-103">tipo de recurso responsáveis</span><span class="sxs-lookup"><span data-stu-id="81f37-103">custodian resource type</span></span>

<span data-ttu-id="81f37-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="81f37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81f37-105">No contexto da descoberta eletrônica, representa um usuário e todos os seus ativos digitais, como emails e documentos.</span><span class="sxs-lookup"><span data-stu-id="81f37-105">In the context of eDiscovery, represents a user and all of their digital assets, such as email and documents.</span></span>

## <a name="methods"></a><span data-ttu-id="81f37-106">Methods</span><span class="sxs-lookup"><span data-stu-id="81f37-106">Methods</span></span>

|<span data-ttu-id="81f37-107">Método</span><span class="sxs-lookup"><span data-stu-id="81f37-107">Method</span></span>|<span data-ttu-id="81f37-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="81f37-108">Return type</span></span>|<span data-ttu-id="81f37-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="81f37-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81f37-110">Listar os responsáveis</span><span class="sxs-lookup"><span data-stu-id="81f37-110">List custodians</span></span>](../api/ediscoverycase-list-custodians.md)|<span data-ttu-id="81f37-111">coleção [responsáveis](../resources/custodian.md)</span><span class="sxs-lookup"><span data-stu-id="81f37-111">[custodian](../resources/custodian.md) collection</span></span>|<span data-ttu-id="81f37-112">Obter uma lista de objetos **responsáveis** e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="81f37-112">Get a list of **custodian** objects and their properties.</span></span>|
|[<span data-ttu-id="81f37-113">Criar responsáveis</span><span class="sxs-lookup"><span data-stu-id="81f37-113">Create custodian</span></span>](../api/ediscoverycase-post-custodians.md)|[<span data-ttu-id="81f37-114">custódia</span><span class="sxs-lookup"><span data-stu-id="81f37-114">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="81f37-115">Criar um novo objeto de **responsáveis** .</span><span class="sxs-lookup"><span data-stu-id="81f37-115">Create a new **custodian** object.</span></span>|
|[<span data-ttu-id="81f37-116">Obter os responsáveis</span><span class="sxs-lookup"><span data-stu-id="81f37-116">Get custodian</span></span>](../api/custodian-get.md)|[<span data-ttu-id="81f37-117">custódia</span><span class="sxs-lookup"><span data-stu-id="81f37-117">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="81f37-118">Leia as propriedades e os relacionamentos de um objeto de **responsáveis** .</span><span class="sxs-lookup"><span data-stu-id="81f37-118">Read the properties and relationships of a **custodian** object.</span></span>|
|[<span data-ttu-id="81f37-119">Atualizar responsáveis</span><span class="sxs-lookup"><span data-stu-id="81f37-119">Update custodian</span></span>](../api/custodian-update.md)|[<span data-ttu-id="81f37-120">custódia</span><span class="sxs-lookup"><span data-stu-id="81f37-120">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="81f37-121">Atualizar as propriedades de um objeto de **responsáveis** .</span><span class="sxs-lookup"><span data-stu-id="81f37-121">Update the properties of a **custodian** object.</span></span>|
|[<span data-ttu-id="81f37-122">comunicado</span><span class="sxs-lookup"><span data-stu-id="81f37-122">release</span></span>](../api/custodian-release.md)|<span data-ttu-id="81f37-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81f37-123">None</span></span>|<span data-ttu-id="81f37-124">Liberar um dos casos.</span><span class="sxs-lookup"><span data-stu-id="81f37-124">Release a custodian from a case.</span></span>|
|[<span data-ttu-id="81f37-125">ativar</span><span class="sxs-lookup"><span data-stu-id="81f37-125">activate</span></span>](../api/custodian-activate.md)|<span data-ttu-id="81f37-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81f37-126">None</span></span>|<span data-ttu-id="81f37-127">Reative os responsáveis que foram liberados de um caso e torne-os parte do caso novamente.</span><span class="sxs-lookup"><span data-stu-id="81f37-127">Reactivate a custodian that has been released from a case and make them part of the case again.</span></span>|
|[<span data-ttu-id="81f37-128">Listar siteSources</span><span class="sxs-lookup"><span data-stu-id="81f37-128">List siteSources</span></span>](../api/custodian-list-sitesources.md)|<span data-ttu-id="81f37-129">coleção de [sites de site](../resources/sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="81f37-129">[siteSource](../resources/sitesource.md) collection</span></span>|<span data-ttu-id="81f37-130">Obtenha os recursos de **site** da propriedade de navegação **siteSources** .</span><span class="sxs-lookup"><span data-stu-id="81f37-130">Get the **siteSource** resources from the **siteSources** navigation property.</span></span>|
|[<span data-ttu-id="81f37-131">Criar siteSources</span><span class="sxs-lookup"><span data-stu-id="81f37-131">Create siteSources</span></span>](../api/custodian-post-sitesources.md)|[<span data-ttu-id="81f37-132">site da site</span><span class="sxs-lookup"><span data-stu-id="81f37-132">siteSource</span></span>](../resources/sitesource.md)|<span data-ttu-id="81f37-133">Criar um novo objeto **sitery** .</span><span class="sxs-lookup"><span data-stu-id="81f37-133">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="81f37-134">Listar unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="81f37-134">List unifiedGroupSources</span></span>](../api/custodian-list-unifiedgroupsources.md)|<span data-ttu-id="81f37-135">coleção [unifiedGroupSource](../resources/unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="81f37-135">[unifiedGroupSource](../resources/unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="81f37-136">Obtenha os recursos **unifiedGroupSource** da propriedade de navegação **unifiedGroupSources** .</span><span class="sxs-lookup"><span data-stu-id="81f37-136">Get the **unifiedGroupSource** resources from the **unifiedGroupSources** navigation property.</span></span>|
|[<span data-ttu-id="81f37-137">Criar unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="81f37-137">Create unifiedGroupSources</span></span>](../api/custodian-post-unifiedgroupsources.md)|[<span data-ttu-id="81f37-138">unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="81f37-138">unifiedGroupSource</span></span>](../resources/unifiedgroupsource.md)|<span data-ttu-id="81f37-139">Criar um novo objeto **unifiedGroupSource** .</span><span class="sxs-lookup"><span data-stu-id="81f37-139">Create a new **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="81f37-140">Listar usersources</span><span class="sxs-lookup"><span data-stu-id="81f37-140">List userSources</span></span>](../api/custodian-list-usersources.md)|<span data-ttu-id="81f37-141">coleção [username](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="81f37-141">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="81f37-142">Obter os recursos de **username** da propriedade de navegação **usersources** .</span><span class="sxs-lookup"><span data-stu-id="81f37-142">Get the **userSource** resources from the **userSources** navigation property.</span></span>|
|[<span data-ttu-id="81f37-143">Criar usersources</span><span class="sxs-lookup"><span data-stu-id="81f37-143">Create userSources</span></span>](../api/custodian-post-usersources.md)|[<span data-ttu-id="81f37-144">username</span><span class="sxs-lookup"><span data-stu-id="81f37-144">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="81f37-145">Criar um novo objeto **username** .</span><span class="sxs-lookup"><span data-stu-id="81f37-145">Create a new **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="81f37-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81f37-146">Properties</span></span>

|<span data-ttu-id="81f37-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81f37-147">Property</span></span>|<span data-ttu-id="81f37-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="81f37-148">Type</span></span>|<span data-ttu-id="81f37-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="81f37-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81f37-150">acknowledgedDateTime</span><span class="sxs-lookup"><span data-stu-id="81f37-150">acknowledgedDateTime</span></span>|<span data-ttu-id="81f37-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81f37-151">DateTimeOffset</span></span>|<span data-ttu-id="81f37-152">Data e hora em que os responsáveis confirmaram uma notificação de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="81f37-152">Date and time the custodian acknowledged a hold notification.</span></span>|
|<span data-ttu-id="81f37-153">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="81f37-153">applyHoldToSources</span></span>|<span data-ttu-id="81f37-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="81f37-154">Boolean</span></span>|<span data-ttu-id="81f37-155">Identifica se as fontes dos responsáveis foram colocadas em espera durante a criação.</span><span class="sxs-lookup"><span data-stu-id="81f37-155">Identifies whether a custodian's sources were placed on hold during creation.</span></span>|
|<span data-ttu-id="81f37-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81f37-156">createdDateTime</span></span>|<span data-ttu-id="81f37-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81f37-157">DateTimeOffset</span></span>|<span data-ttu-id="81f37-158">Data e hora em que os responsáveis foram adicionados ao caso.</span><span class="sxs-lookup"><span data-stu-id="81f37-158">Date and time when the custodian was added to the case.</span></span>|
|<span data-ttu-id="81f37-159">displayName</span><span class="sxs-lookup"><span data-stu-id="81f37-159">displayName</span></span>|<span data-ttu-id="81f37-160">String</span><span class="sxs-lookup"><span data-stu-id="81f37-160">String</span></span>|<span data-ttu-id="81f37-161">Nome de exibição do responsáveis.</span><span class="sxs-lookup"><span data-stu-id="81f37-161">Display name of the custodian.</span></span>|
|<span data-ttu-id="81f37-162">email</span><span class="sxs-lookup"><span data-stu-id="81f37-162">email</span></span>|<span data-ttu-id="81f37-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81f37-163">String</span></span>|<span data-ttu-id="81f37-164">Endereço de email do responsáveis.</span><span class="sxs-lookup"><span data-stu-id="81f37-164">Email address of the custodian.</span></span>|
|<span data-ttu-id="81f37-165">id</span><span class="sxs-lookup"><span data-stu-id="81f37-165">id</span></span>|<span data-ttu-id="81f37-166">String</span><span class="sxs-lookup"><span data-stu-id="81f37-166">String</span></span>|<span data-ttu-id="81f37-167">A ID dos responsáveis no caso especificado.</span><span class="sxs-lookup"><span data-stu-id="81f37-167">The ID for the custodian in the specified case.</span></span> <span data-ttu-id="81f37-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81f37-168">Read-only.</span></span>|
|<span data-ttu-id="81f37-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81f37-169">lastModifiedDateTime</span></span>|<span data-ttu-id="81f37-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81f37-170">DateTimeOffset</span></span>|<span data-ttu-id="81f37-171">Data e hora da última modificação do objeto responsáveis</span><span class="sxs-lookup"><span data-stu-id="81f37-171">Date and time the custodian object was last modified</span></span>|
|<span data-ttu-id="81f37-172">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="81f37-172">releasedDateTime</span></span>|<span data-ttu-id="81f37-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81f37-173">DateTimeOffset</span></span>|<span data-ttu-id="81f37-174">Data e hora em que os responsáveis foram liberados do caso.</span><span class="sxs-lookup"><span data-stu-id="81f37-174">Date and time the custodian was released from the case.</span></span>|
|<span data-ttu-id="81f37-175">status</span><span class="sxs-lookup"><span data-stu-id="81f37-175">status</span></span>|<span data-ttu-id="81f37-176">custodianStatus</span><span class="sxs-lookup"><span data-stu-id="81f37-176">custodianStatus</span></span>|<span data-ttu-id="81f37-177">Status dos responsáveis.</span><span class="sxs-lookup"><span data-stu-id="81f37-177">Status of the custodian.</span></span> <span data-ttu-id="81f37-178">Os valores possíveis são: `active` e `released`.</span><span class="sxs-lookup"><span data-stu-id="81f37-178">Possible values are: `active`, `released`.</span></span>|

### <a name="custodianstatus-values"></a><span data-ttu-id="81f37-179">valores de custodianStatus</span><span class="sxs-lookup"><span data-stu-id="81f37-179">custodianStatus values</span></span>

|<span data-ttu-id="81f37-180">Member</span><span class="sxs-lookup"><span data-stu-id="81f37-180">Member</span></span>|<span data-ttu-id="81f37-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="81f37-181">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="81f37-182">active</span><span class="sxs-lookup"><span data-stu-id="81f37-182">active</span></span>|<span data-ttu-id="81f37-183">O responsáveis é uma parte ativa do caso.</span><span class="sxs-lookup"><span data-stu-id="81f37-183">Custodian is an active part of the case.</span></span> |
|<span data-ttu-id="81f37-184">solta</span><span class="sxs-lookup"><span data-stu-id="81f37-184">released</span></span>|<span data-ttu-id="81f37-185">Os responsáveis são liberados do caso.</span><span class="sxs-lookup"><span data-stu-id="81f37-185">Custodian is released from the case.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81f37-186">Relações</span><span class="sxs-lookup"><span data-stu-id="81f37-186">Relationships</span></span>

|<span data-ttu-id="81f37-187">Relação</span><span class="sxs-lookup"><span data-stu-id="81f37-187">Relationship</span></span>|<span data-ttu-id="81f37-188">Tipo</span><span class="sxs-lookup"><span data-stu-id="81f37-188">Type</span></span>|<span data-ttu-id="81f37-189">Descrição</span><span class="sxs-lookup"><span data-stu-id="81f37-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81f37-190">siteSources</span><span class="sxs-lookup"><span data-stu-id="81f37-190">siteSources</span></span>|<span data-ttu-id="81f37-191">coleção de [sites de site](../resources/sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="81f37-191">[siteSource](../resources/sitesource.md) collection</span></span>|<span data-ttu-id="81f37-192">Entidade de fonte de dados para sites do SharePoint associados aos responsáveis.</span><span class="sxs-lookup"><span data-stu-id="81f37-192">Data source entity for SharePoint sites associated with the custodian.</span></span>|
|<span data-ttu-id="81f37-193">unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="81f37-193">unifiedGroupSources</span></span>|<span data-ttu-id="81f37-194">coleção [unifiedGroupSource](../resources/unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="81f37-194">[unifiedGroupSource](../resources/unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="81f37-195">Entidade de fonte de dados para grupos associados aos responsáveis.</span><span class="sxs-lookup"><span data-stu-id="81f37-195">Data source entity for groups associated with the custodian.</span></span>|
|<span data-ttu-id="81f37-196">usersources</span><span class="sxs-lookup"><span data-stu-id="81f37-196">userSources</span></span>|<span data-ttu-id="81f37-197">coleção [username](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="81f37-197">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="81f37-198">Entidade de fonte de dados para um dos responsáveis.</span><span class="sxs-lookup"><span data-stu-id="81f37-198">Data source entity for a the custodian.</span></span> <span data-ttu-id="81f37-199">Este é o contêiner para a caixa de correio de um dos responsáveis e o site do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="81f37-199">This is the container for a custodian's mailbox and OneDrive for Business site.</span></span>|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a><span data-ttu-id="81f37-200">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81f37-200">JSON representation</span></span>

<span data-ttu-id="81f37-201">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81f37-201">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.custodian",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.custodian",
  "email": "String",
  "applyHoldToSources": "Boolean",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "acknowledgedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "displayName": "String"
}
```

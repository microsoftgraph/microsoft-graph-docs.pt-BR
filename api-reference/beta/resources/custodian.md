---
title: tipo de recurso custodian
description: No contexto da Descoberta eDiscovery, representa um usuário e todos os seus ativos digitais, como emails e documentos.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 6c6b2befbb4066b851e38e6e17fd8be5aa59b031
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157677"
---
# <a name="custodian-resource-type"></a><span data-ttu-id="b3fd5-103">tipo de recurso custodian</span><span class="sxs-lookup"><span data-stu-id="b3fd5-103">custodian resource type</span></span>

<span data-ttu-id="b3fd5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3fd5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3fd5-105">No contexto da Descoberta eDiscovery, representa um usuário e todos os seus ativos digitais, como emails e documentos.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-105">In the context of eDiscovery, represents a user and all of their digital assets, such as email and documents.</span></span>

## <a name="methods"></a><span data-ttu-id="b3fd5-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b3fd5-106">Methods</span></span>

|<span data-ttu-id="b3fd5-107">Método</span><span class="sxs-lookup"><span data-stu-id="b3fd5-107">Method</span></span>|<span data-ttu-id="b3fd5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b3fd5-108">Return type</span></span>|<span data-ttu-id="b3fd5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3fd5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b3fd5-110">Listar custodiantes</span><span class="sxs-lookup"><span data-stu-id="b3fd5-110">List custodians</span></span>](../api/ediscoverycase-list-custodians.md)|<span data-ttu-id="b3fd5-111">[coleção custodian](../resources/custodian.md)</span><span class="sxs-lookup"><span data-stu-id="b3fd5-111">[custodian](../resources/custodian.md) collection</span></span>|<span data-ttu-id="b3fd5-112">Obter uma lista de **objetos custodiantes** e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-112">Get a list of **custodian** objects and their properties.</span></span>|
|[<span data-ttu-id="b3fd5-113">Criar custodiatário</span><span class="sxs-lookup"><span data-stu-id="b3fd5-113">Create custodian</span></span>](../api/ediscoverycase-post-custodians.md)|[<span data-ttu-id="b3fd5-114">custodian</span><span class="sxs-lookup"><span data-stu-id="b3fd5-114">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="b3fd5-115">Criar um novo **objeto custodiante.**</span><span class="sxs-lookup"><span data-stu-id="b3fd5-115">Create a new **custodian** object.</span></span>|
|[<span data-ttu-id="b3fd5-116">Obter custodian</span><span class="sxs-lookup"><span data-stu-id="b3fd5-116">Get custodian</span></span>](../api/custodian-get.md)|[<span data-ttu-id="b3fd5-117">custodian</span><span class="sxs-lookup"><span data-stu-id="b3fd5-117">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="b3fd5-118">Leia as propriedades e os relacionamentos de um **objeto custodiante.**</span><span class="sxs-lookup"><span data-stu-id="b3fd5-118">Read the properties and relationships of a **custodian** object.</span></span>|
|[<span data-ttu-id="b3fd5-119">Atualizar custodian</span><span class="sxs-lookup"><span data-stu-id="b3fd5-119">Update custodian</span></span>](../api/custodian-update.md)|[<span data-ttu-id="b3fd5-120">custodian</span><span class="sxs-lookup"><span data-stu-id="b3fd5-120">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="b3fd5-121">Atualizar as propriedades de **um objeto custodiante.**</span><span class="sxs-lookup"><span data-stu-id="b3fd5-121">Update the properties of a **custodian** object.</span></span>|
|[<span data-ttu-id="b3fd5-122">release</span><span class="sxs-lookup"><span data-stu-id="b3fd5-122">release</span></span>](../api/custodian-release.md)|<span data-ttu-id="b3fd5-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="b3fd5-123">None</span></span>|<span data-ttu-id="b3fd5-124">Libere um custodiante de uma ocorrência.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-124">Release a custodian from a case.</span></span>|
|[<span data-ttu-id="b3fd5-125">ativar</span><span class="sxs-lookup"><span data-stu-id="b3fd5-125">activate</span></span>](../api/custodian-activate.md)|<span data-ttu-id="b3fd5-126">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="b3fd5-126">None</span></span>|<span data-ttu-id="b3fd5-127">Reativar um custodiante que foi liberado de uma ocorrência e torná-lo parte do caso novamente.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-127">Reactivate a custodian that has been released from a case and make them part of the case again.</span></span>|
|[<span data-ttu-id="b3fd5-128">Listar siteSources</span><span class="sxs-lookup"><span data-stu-id="b3fd5-128">List siteSources</span></span>](../api/custodian-list-sitesources.md)|<span data-ttu-id="b3fd5-129">[coleção siteSource](../resources/sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="b3fd5-129">[siteSource](../resources/sitesource.md) collection</span></span>|<span data-ttu-id="b3fd5-130">Obter os **recursos siteSource** da **propriedade de navegação siteSources.**</span><span class="sxs-lookup"><span data-stu-id="b3fd5-130">Get the **siteSource** resources from the **siteSources** navigation property.</span></span>|
|[<span data-ttu-id="b3fd5-131">Criar siteSources</span><span class="sxs-lookup"><span data-stu-id="b3fd5-131">Create siteSources</span></span>](../api/custodian-post-sitesources.md)|[<span data-ttu-id="b3fd5-132">siteSource</span><span class="sxs-lookup"><span data-stu-id="b3fd5-132">siteSource</span></span>](../resources/sitesource.md)|<span data-ttu-id="b3fd5-133">Criar um novo **objeto siteSource.**</span><span class="sxs-lookup"><span data-stu-id="b3fd5-133">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="b3fd5-134">Listar unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="b3fd5-134">List unifiedGroupSources</span></span>](../api/custodian-list-unifiedgroupsources.md)|<span data-ttu-id="b3fd5-135">[Coleção unifiedGroupSource](../resources/unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="b3fd5-135">[unifiedGroupSource](../resources/unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="b3fd5-136">Obter os **recursos unifiedGroupSource** da **propriedade de navegação unifiedGroupSources.**</span><span class="sxs-lookup"><span data-stu-id="b3fd5-136">Get the **unifiedGroupSource** resources from the **unifiedGroupSources** navigation property.</span></span>|
|[<span data-ttu-id="b3fd5-137">Criar unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="b3fd5-137">Create unifiedGroupSources</span></span>](../api/custodian-post-unifiedgroupsources.md)|[<span data-ttu-id="b3fd5-138">unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="b3fd5-138">unifiedGroupSource</span></span>](../resources/unifiedgroupsource.md)|<span data-ttu-id="b3fd5-139">Crie um novo **objeto unifiedGroupSource.**</span><span class="sxs-lookup"><span data-stu-id="b3fd5-139">Create a new **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="b3fd5-140">Listar userSources</span><span class="sxs-lookup"><span data-stu-id="b3fd5-140">List userSources</span></span>](../api/custodian-list-usersources.md)|<span data-ttu-id="b3fd5-141">[Coleção userSource](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="b3fd5-141">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="b3fd5-142">Obter os **recursos userSource** da **propriedade de navegação userSources.**</span><span class="sxs-lookup"><span data-stu-id="b3fd5-142">Get the **userSource** resources from the **userSources** navigation property.</span></span>|
|[<span data-ttu-id="b3fd5-143">Criar userSources</span><span class="sxs-lookup"><span data-stu-id="b3fd5-143">Create userSources</span></span>](../api/custodian-post-usersources.md)|[<span data-ttu-id="b3fd5-144">userSource</span><span class="sxs-lookup"><span data-stu-id="b3fd5-144">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="b3fd5-145">Crie um novo **objeto userSource.**</span><span class="sxs-lookup"><span data-stu-id="b3fd5-145">Create a new **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3fd5-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3fd5-146">Properties</span></span>

|<span data-ttu-id="b3fd5-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3fd5-147">Property</span></span>|<span data-ttu-id="b3fd5-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3fd5-148">Type</span></span>|<span data-ttu-id="b3fd5-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3fd5-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3fd5-150">acknowledgedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3fd5-150">acknowledgedDateTime</span></span>|<span data-ttu-id="b3fd5-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3fd5-151">DateTimeOffset</span></span>|<span data-ttu-id="b3fd5-152">Data e hora em que o custodiado reconheceu uma notificação de espera.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-152">Date and time the custodian acknowledged a hold notification.</span></span>|
|<span data-ttu-id="b3fd5-153">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="b3fd5-153">applyHoldToSources</span></span>|<span data-ttu-id="b3fd5-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3fd5-154">Boolean</span></span>|<span data-ttu-id="b3fd5-155">Identifica se as fontes de um custodiador foram colocadas em espera durante a criação.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-155">Identifies whether a custodian's sources were placed on hold during creation.</span></span>|
|<span data-ttu-id="b3fd5-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3fd5-156">createdDateTime</span></span>|<span data-ttu-id="b3fd5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3fd5-157">DateTimeOffset</span></span>|<span data-ttu-id="b3fd5-158">Data e hora em que o custodiante foi adicionado à ocorrência.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-158">Date and time when the custodian was added to the case.</span></span>|
|<span data-ttu-id="b3fd5-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b3fd5-159">displayName</span></span>|<span data-ttu-id="b3fd5-160">String</span><span class="sxs-lookup"><span data-stu-id="b3fd5-160">String</span></span>|<span data-ttu-id="b3fd5-161">Nome de exibição do custodiado.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-161">Display name of the custodian.</span></span>|
|<span data-ttu-id="b3fd5-162">email</span><span class="sxs-lookup"><span data-stu-id="b3fd5-162">email</span></span>|<span data-ttu-id="b3fd5-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3fd5-163">String</span></span>|<span data-ttu-id="b3fd5-164">Endereço de email do custodiatário.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-164">Email address of the custodian.</span></span>|
|<span data-ttu-id="b3fd5-165">id</span><span class="sxs-lookup"><span data-stu-id="b3fd5-165">id</span></span>|<span data-ttu-id="b3fd5-166">String</span><span class="sxs-lookup"><span data-stu-id="b3fd5-166">String</span></span>|<span data-ttu-id="b3fd5-167">A ID do custodiante no caso especificado.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-167">The ID for the custodian in the specified case.</span></span> <span data-ttu-id="b3fd5-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-168">Read-only.</span></span>|
|<span data-ttu-id="b3fd5-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3fd5-169">lastModifiedDateTime</span></span>|<span data-ttu-id="b3fd5-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3fd5-170">DateTimeOffset</span></span>|<span data-ttu-id="b3fd5-171">Data e hora em que o objeto custodiante foi modificado pela última vez</span><span class="sxs-lookup"><span data-stu-id="b3fd5-171">Date and time the custodian object was last modified</span></span>|
|<span data-ttu-id="b3fd5-172">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3fd5-172">releasedDateTime</span></span>|<span data-ttu-id="b3fd5-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3fd5-173">DateTimeOffset</span></span>|<span data-ttu-id="b3fd5-174">Data e hora em que o custodiante foi liberado da ocorrência.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-174">Date and time the custodian was released from the case.</span></span>|
|<span data-ttu-id="b3fd5-175">status</span><span class="sxs-lookup"><span data-stu-id="b3fd5-175">status</span></span>|<span data-ttu-id="b3fd5-176">custodianStatus</span><span class="sxs-lookup"><span data-stu-id="b3fd5-176">custodianStatus</span></span>|<span data-ttu-id="b3fd5-177">Status do custodiatário.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-177">Status of the custodian.</span></span> <span data-ttu-id="b3fd5-178">Os valores possíveis são: `active` e `released`.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-178">Possible values are: `active`, `released`.</span></span>|

### <a name="custodianstatus-values"></a><span data-ttu-id="b3fd5-179">valores de custodianStatus</span><span class="sxs-lookup"><span data-stu-id="b3fd5-179">custodianStatus values</span></span>

|<span data-ttu-id="b3fd5-180">Member</span><span class="sxs-lookup"><span data-stu-id="b3fd5-180">Member</span></span>|<span data-ttu-id="b3fd5-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3fd5-181">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="b3fd5-182">ativo</span><span class="sxs-lookup"><span data-stu-id="b3fd5-182">active</span></span>|<span data-ttu-id="b3fd5-183">Custodian é uma parte ativa da ocorrência.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-183">Custodian is an active part of the case.</span></span> |
|<span data-ttu-id="b3fd5-184">released</span><span class="sxs-lookup"><span data-stu-id="b3fd5-184">released</span></span>|<span data-ttu-id="b3fd5-185">Custodian is released from the case.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-185">Custodian is released from the case.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3fd5-186">Relações</span><span class="sxs-lookup"><span data-stu-id="b3fd5-186">Relationships</span></span>

|<span data-ttu-id="b3fd5-187">Relação</span><span class="sxs-lookup"><span data-stu-id="b3fd5-187">Relationship</span></span>|<span data-ttu-id="b3fd5-188">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3fd5-188">Type</span></span>|<span data-ttu-id="b3fd5-189">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3fd5-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3fd5-190">siteSources</span><span class="sxs-lookup"><span data-stu-id="b3fd5-190">siteSources</span></span>|<span data-ttu-id="b3fd5-191">[coleção siteSource](../resources/sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="b3fd5-191">[siteSource](../resources/sitesource.md) collection</span></span>|<span data-ttu-id="b3fd5-192">Entidade de fonte de dados para sites do SharePoint associados ao custodiante.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-192">Data source entity for SharePoint sites associated with the custodian.</span></span>|
|<span data-ttu-id="b3fd5-193">unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="b3fd5-193">unifiedGroupSources</span></span>|<span data-ttu-id="b3fd5-194">[Coleção unifiedGroupSource](../resources/unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="b3fd5-194">[unifiedGroupSource](../resources/unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="b3fd5-195">Entidade de fonte de dados para grupos associados ao custodiante.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-195">Data source entity for groups associated with the custodian.</span></span>|
|<span data-ttu-id="b3fd5-196">userSources</span><span class="sxs-lookup"><span data-stu-id="b3fd5-196">userSources</span></span>|<span data-ttu-id="b3fd5-197">[Coleção userSource](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="b3fd5-197">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="b3fd5-198">Entidade de fonte de dados para um custodiante.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-198">Data source entity for a the custodian.</span></span> <span data-ttu-id="b3fd5-199">Esse é o contêiner da caixa de correio de um responsável e do site do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-199">This is the container for a custodian's mailbox and OneDrive for Business site.</span></span>|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a><span data-ttu-id="b3fd5-200">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3fd5-200">JSON representation</span></span>

<span data-ttu-id="b3fd5-201">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3fd5-201">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.custodian",
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

---
title: Atualizar windowsFeatureUpdateCatalogItem
description: Atualizar as propriedades de um objeto windowsFeatureUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 54603daa0498ede2db73705daac09655da64fbf5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160124"
---
# <a name="update-windowsfeatureupdatecatalogitem"></a><span data-ttu-id="fdf69-103">Atualizar windowsFeatureUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="fdf69-103">Update windowsFeatureUpdateCatalogItem</span></span>

<span data-ttu-id="fdf69-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdf69-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fdf69-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fdf69-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdf69-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fdf69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdf69-107">Atualizar as propriedades de um [objeto windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="fdf69-107">Update the properties of a [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdf69-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fdf69-108">Prerequisites</span></span>
<span data-ttu-id="fdf69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdf69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdf69-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdf69-111">Permission type</span></span>|<span data-ttu-id="fdf69-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fdf69-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdf69-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdf69-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdf69-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdf69-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fdf69-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdf69-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdf69-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdf69-116">Not supported.</span></span>|
|<span data-ttu-id="fdf69-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdf69-117">Application</span></span>|<span data-ttu-id="fdf69-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdf69-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdf69-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdf69-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

## <a name="request-headers"></a><span data-ttu-id="fdf69-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdf69-120">Request headers</span></span>
|<span data-ttu-id="fdf69-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fdf69-121">Header</span></span>|<span data-ttu-id="fdf69-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fdf69-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdf69-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdf69-123">Authorization</span></span>|<span data-ttu-id="fdf69-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdf69-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdf69-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fdf69-125">Accept</span></span>|<span data-ttu-id="fdf69-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdf69-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdf69-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdf69-127">Request body</span></span>
<span data-ttu-id="fdf69-128">No corpo da solicitação, fornece uma representação JSON do [objeto windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="fdf69-128">In the request body, supply a JSON representation for the [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object.</span></span>

<span data-ttu-id="fdf69-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md).</span><span class="sxs-lookup"><span data-stu-id="fdf69-129">The following table shows the properties that are required when you create the [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md).</span></span>

|<span data-ttu-id="fdf69-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdf69-130">Property</span></span>|<span data-ttu-id="fdf69-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdf69-131">Type</span></span>|<span data-ttu-id="fdf69-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdf69-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdf69-133">id</span><span class="sxs-lookup"><span data-stu-id="fdf69-133">id</span></span>|<span data-ttu-id="fdf69-134">String</span><span class="sxs-lookup"><span data-stu-id="fdf69-134">String</span></span>|<span data-ttu-id="fdf69-135">A ID do item de catálogo. Herdado [de windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="fdf69-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="fdf69-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fdf69-136">displayName</span></span>|<span data-ttu-id="fdf69-137">String</span><span class="sxs-lookup"><span data-stu-id="fdf69-137">String</span></span>|<span data-ttu-id="fdf69-138">O nome de exibição do item de catálogo.</span><span class="sxs-lookup"><span data-stu-id="fdf69-138">The display name for the catalog item.</span></span> <span data-ttu-id="fdf69-139">Herdado [de windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="fdf69-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="fdf69-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="fdf69-140">releaseDateTime</span></span>|<span data-ttu-id="fdf69-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdf69-141">DateTimeOffset</span></span>|<span data-ttu-id="fdf69-142">A data em que o item de catálogo foi lançado Herdado de [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="fdf69-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="fdf69-143">versão</span><span class="sxs-lookup"><span data-stu-id="fdf69-143">version</span></span>|<span data-ttu-id="fdf69-144">String</span><span class="sxs-lookup"><span data-stu-id="fdf69-144">String</span></span>|<span data-ttu-id="fdf69-145">A versão de atualização de recursos</span><span class="sxs-lookup"><span data-stu-id="fdf69-145">The feature update version</span></span>|



## <a name="response"></a><span data-ttu-id="fdf69-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdf69-146">Response</span></span>
<span data-ttu-id="fdf69-147">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdf69-147">If successful, this method returns a `200 OK` response code and an updated [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdf69-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdf69-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdf69-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdf69-149">Request</span></span>
<span data-ttu-id="fdf69-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdf69-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
Content-type: application/json
Content-length: 203

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="fdf69-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdf69-151">Response</span></span>
<span data-ttu-id="fdf69-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdf69-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 252

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "id": "cbd85729-5729-cbd8-2957-d8cb2957d8cb",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "version": "Version value"
}
```





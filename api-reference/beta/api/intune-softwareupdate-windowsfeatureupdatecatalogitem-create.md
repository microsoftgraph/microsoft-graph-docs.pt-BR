---
title: Criar windowsFeatureUpdateCatalogItem
description: Crie um novo objeto windowsFeatureUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3b7cf68452f5b1c2a0b6d8b4df3a06554e4faae7
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866934"
---
# <a name="create-windowsfeatureupdatecatalogitem"></a><span data-ttu-id="15f9f-103">Criar windowsFeatureUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="15f9f-103">Create windowsFeatureUpdateCatalogItem</span></span>

<span data-ttu-id="15f9f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15f9f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15f9f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="15f9f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15f9f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15f9f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15f9f-107">Crie um novo [objeto windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="15f9f-107">Create a new [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15f9f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15f9f-108">Prerequisites</span></span>
<span data-ttu-id="15f9f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15f9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15f9f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15f9f-111">Permission type</span></span>|<span data-ttu-id="15f9f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15f9f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15f9f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15f9f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15f9f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15f9f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15f9f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15f9f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15f9f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15f9f-116">Not supported.</span></span>|
|<span data-ttu-id="15f9f-117">Application</span><span class="sxs-lookup"><span data-stu-id="15f9f-117">Application</span></span>|<span data-ttu-id="15f9f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15f9f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15f9f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15f9f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="15f9f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15f9f-120">Request headers</span></span>
|<span data-ttu-id="15f9f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15f9f-121">Header</span></span>|<span data-ttu-id="15f9f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="15f9f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15f9f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="15f9f-123">Authorization</span></span>|<span data-ttu-id="15f9f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15f9f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15f9f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15f9f-125">Accept</span></span>|<span data-ttu-id="15f9f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15f9f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15f9f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15f9f-127">Request body</span></span>
<span data-ttu-id="15f9f-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsFeatureUpdateCatalogItem.</span><span class="sxs-lookup"><span data-stu-id="15f9f-128">In the request body, supply a JSON representation for the windowsFeatureUpdateCatalogItem object.</span></span>

<span data-ttu-id="15f9f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o windowsFeatureUpdateCatalogItem.</span><span class="sxs-lookup"><span data-stu-id="15f9f-129">The following table shows the properties that are required when you create the windowsFeatureUpdateCatalogItem.</span></span>

|<span data-ttu-id="15f9f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15f9f-130">Property</span></span>|<span data-ttu-id="15f9f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="15f9f-131">Type</span></span>|<span data-ttu-id="15f9f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="15f9f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15f9f-133">id</span><span class="sxs-lookup"><span data-stu-id="15f9f-133">id</span></span>|<span data-ttu-id="15f9f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15f9f-134">String</span></span>|<span data-ttu-id="15f9f-135">A ID do item de catálogo. Herdado [do windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="15f9f-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="15f9f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="15f9f-136">displayName</span></span>|<span data-ttu-id="15f9f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15f9f-137">String</span></span>|<span data-ttu-id="15f9f-138">O nome de exibição do item de catálogo.</span><span class="sxs-lookup"><span data-stu-id="15f9f-138">The display name for the catalog item.</span></span> <span data-ttu-id="15f9f-139">Herdado [do windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="15f9f-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="15f9f-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="15f9f-140">releaseDateTime</span></span>|<span data-ttu-id="15f9f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15f9f-141">DateTimeOffset</span></span>|<span data-ttu-id="15f9f-142">A data em que o item de catálogo foi lançado Herdado de [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="15f9f-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="15f9f-143">endOfSupportDate</span><span class="sxs-lookup"><span data-stu-id="15f9f-143">endOfSupportDate</span></span>|<span data-ttu-id="15f9f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15f9f-144">DateTimeOffset</span></span>|<span data-ttu-id="15f9f-145">A última data com suporte para um item de catálogo Herdado de [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="15f9f-145">The last supported date for a catalog item Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="15f9f-146">versão</span><span class="sxs-lookup"><span data-stu-id="15f9f-146">version</span></span>|<span data-ttu-id="15f9f-147">String</span><span class="sxs-lookup"><span data-stu-id="15f9f-147">String</span></span>|<span data-ttu-id="15f9f-148">A versão de atualização de recursos</span><span class="sxs-lookup"><span data-stu-id="15f9f-148">The feature update version</span></span>|



## <a name="response"></a><span data-ttu-id="15f9f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f9f-149">Response</span></span>
<span data-ttu-id="15f9f-150">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15f9f-150">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15f9f-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15f9f-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="15f9f-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15f9f-152">Request</span></span>
<span data-ttu-id="15f9f-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15f9f-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
Content-type: application/json
Content-length: 263

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="15f9f-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f9f-154">Response</span></span>
<span data-ttu-id="15f9f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15f9f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 312

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "id": "cbd85729-5729-cbd8-2957-d8cb2957d8cb",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00",
  "version": "Version value"
}
```





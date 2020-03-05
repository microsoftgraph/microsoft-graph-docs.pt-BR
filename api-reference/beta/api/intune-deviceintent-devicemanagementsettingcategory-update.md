---
title: Atualizar deviceManagementSettingCategory
description: Atualiza as propriedades de um objeto deviceManagementSettingCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7a2b6e815fb96ca14c78be467921c9926d8e4bba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470599"
---
# <a name="update-devicemanagementsettingcategory"></a><span data-ttu-id="bca6a-103">Atualizar deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="bca6a-103">Update deviceManagementSettingCategory</span></span>

<span data-ttu-id="bca6a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bca6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bca6a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bca6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bca6a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bca6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bca6a-107">Atualiza as propriedades de um objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="bca6a-107">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bca6a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bca6a-108">Prerequisites</span></span>
<span data-ttu-id="bca6a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bca6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bca6a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bca6a-111">Permission type</span></span>|<span data-ttu-id="bca6a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bca6a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bca6a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bca6a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bca6a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bca6a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bca6a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bca6a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bca6a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bca6a-116">Not supported.</span></span>|
|<span data-ttu-id="bca6a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bca6a-117">Application</span></span>|<span data-ttu-id="bca6a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bca6a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bca6a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bca6a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="bca6a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bca6a-120">Request headers</span></span>
|<span data-ttu-id="bca6a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bca6a-121">Header</span></span>|<span data-ttu-id="bca6a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bca6a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bca6a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bca6a-123">Authorization</span></span>|<span data-ttu-id="bca6a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bca6a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bca6a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bca6a-125">Accept</span></span>|<span data-ttu-id="bca6a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bca6a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bca6a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bca6a-127">Request body</span></span>
<span data-ttu-id="bca6a-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="bca6a-128">In the request body, supply a JSON representation for the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

<span data-ttu-id="bca6a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span><span class="sxs-lookup"><span data-stu-id="bca6a-129">The following table shows the properties that are required when you create the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>

|<span data-ttu-id="bca6a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bca6a-130">Property</span></span>|<span data-ttu-id="bca6a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bca6a-131">Type</span></span>|<span data-ttu-id="bca6a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bca6a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bca6a-133">id</span><span class="sxs-lookup"><span data-stu-id="bca6a-133">id</span></span>|<span data-ttu-id="bca6a-134">String</span><span class="sxs-lookup"><span data-stu-id="bca6a-134">String</span></span>|<span data-ttu-id="bca6a-135">A ID da categoria</span><span class="sxs-lookup"><span data-stu-id="bca6a-135">The category ID</span></span>|
|<span data-ttu-id="bca6a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bca6a-136">displayName</span></span>|<span data-ttu-id="bca6a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bca6a-137">String</span></span>|<span data-ttu-id="bca6a-138">O nome da categoria</span><span class="sxs-lookup"><span data-stu-id="bca6a-138">The category name</span></span>|
|<span data-ttu-id="bca6a-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="bca6a-139">hasRequiredSetting</span></span>|<span data-ttu-id="bca6a-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="bca6a-140">Boolean</span></span>|<span data-ttu-id="bca6a-141">A categoria contém a configuração necessária de nível superior</span><span class="sxs-lookup"><span data-stu-id="bca6a-141">The category contains top level required setting</span></span>|



## <a name="response"></a><span data-ttu-id="bca6a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="bca6a-142">Response</span></span>
<span data-ttu-id="bca6a-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bca6a-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bca6a-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bca6a-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="bca6a-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bca6a-145">Request</span></span>
<span data-ttu-id="bca6a-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bca6a-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/categories/{deviceManagementSettingCategoryId}
Content-type: application/json
Content-length: 144

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="bca6a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="bca6a-147">Response</span></span>
<span data-ttu-id="bca6a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bca6a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 193

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```






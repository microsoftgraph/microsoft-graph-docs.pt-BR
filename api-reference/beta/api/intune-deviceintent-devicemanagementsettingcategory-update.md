---
title: Atualizar deviceManagementSettingCategory
description: Atualiza as propriedades de um objeto deviceManagementSettingCategory.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a4e5711e8d9adf026e94b85c01c0d7e384ce677c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815104"
---
# <a name="update-devicemanagementsettingcategory"></a><span data-ttu-id="f079f-103">Atualizar deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="f079f-103">Update deviceManagementSettingCategory</span></span>

> <span data-ttu-id="f079f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f079f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f079f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f079f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f079f-106">Atualiza as propriedades de um objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="f079f-106">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f079f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f079f-107">Prerequisites</span></span>
<span data-ttu-id="f079f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f079f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f079f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f079f-110">Permission type</span></span>|<span data-ttu-id="f079f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f079f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f079f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f079f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f079f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f079f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f079f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f079f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f079f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f079f-115">Not supported.</span></span>|
|<span data-ttu-id="f079f-116">Application</span><span class="sxs-lookup"><span data-stu-id="f079f-116">Application</span></span>|<span data-ttu-id="f079f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f079f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f079f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f079f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="f079f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f079f-119">Request headers</span></span>
|<span data-ttu-id="f079f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f079f-120">Header</span></span>|<span data-ttu-id="f079f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f079f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f079f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f079f-122">Authorization</span></span>|<span data-ttu-id="f079f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f079f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f079f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f079f-124">Accept</span></span>|<span data-ttu-id="f079f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f079f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f079f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f079f-126">Request body</span></span>
<span data-ttu-id="f079f-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="f079f-127">In the request body, supply a JSON representation for the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

<span data-ttu-id="f079f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span><span class="sxs-lookup"><span data-stu-id="f079f-128">The following table shows the properties that are required when you create the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>

|<span data-ttu-id="f079f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f079f-129">Property</span></span>|<span data-ttu-id="f079f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f079f-130">Type</span></span>|<span data-ttu-id="f079f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f079f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f079f-132">id</span><span class="sxs-lookup"><span data-stu-id="f079f-132">id</span></span>|<span data-ttu-id="f079f-133">String</span><span class="sxs-lookup"><span data-stu-id="f079f-133">String</span></span>|<span data-ttu-id="f079f-134">A ID da categoria</span><span class="sxs-lookup"><span data-stu-id="f079f-134">The category ID</span></span>|
|<span data-ttu-id="f079f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f079f-135">displayName</span></span>|<span data-ttu-id="f079f-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f079f-136">String</span></span>|<span data-ttu-id="f079f-137">O nome da categoria</span><span class="sxs-lookup"><span data-stu-id="f079f-137">The category name</span></span>|
|<span data-ttu-id="f079f-138">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="f079f-138">hasRequiredSetting</span></span>|<span data-ttu-id="f079f-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="f079f-139">Boolean</span></span>|<span data-ttu-id="f079f-140">A categoria contém a configuração necessária de nível superior</span><span class="sxs-lookup"><span data-stu-id="f079f-140">The category contains top level required setting</span></span>|



## <a name="response"></a><span data-ttu-id="f079f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f079f-141">Response</span></span>
<span data-ttu-id="f079f-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f079f-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f079f-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f079f-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="f079f-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f079f-144">Request</span></span>
<span data-ttu-id="f079f-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f079f-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f079f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f079f-146">Response</span></span>
<span data-ttu-id="f079f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f079f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





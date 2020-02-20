---
title: Atualizar deviceManagementSettingCategory
description: Atualiza as propriedades de um objeto deviceManagementSettingCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58bda115444b78ee414b2d6a445ab97b489736d0
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162292"
---
# <a name="update-devicemanagementsettingcategory"></a><span data-ttu-id="7d125-103">Atualizar deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="7d125-103">Update deviceManagementSettingCategory</span></span>

> <span data-ttu-id="7d125-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7d125-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d125-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d125-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d125-106">Atualiza as propriedades de um objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="7d125-106">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d125-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d125-107">Prerequisites</span></span>
<span data-ttu-id="7d125-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d125-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d125-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d125-110">Permission type</span></span>|<span data-ttu-id="7d125-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d125-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d125-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d125-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d125-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d125-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d125-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d125-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d125-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d125-115">Not supported.</span></span>|
|<span data-ttu-id="7d125-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d125-116">Application</span></span>|<span data-ttu-id="7d125-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d125-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d125-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d125-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="7d125-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d125-119">Request headers</span></span>
|<span data-ttu-id="7d125-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d125-120">Header</span></span>|<span data-ttu-id="7d125-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7d125-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d125-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d125-122">Authorization</span></span>|<span data-ttu-id="7d125-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d125-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d125-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d125-124">Accept</span></span>|<span data-ttu-id="7d125-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7d125-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d125-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d125-126">Request body</span></span>
<span data-ttu-id="7d125-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="7d125-127">In the request body, supply a JSON representation for the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

<span data-ttu-id="7d125-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span><span class="sxs-lookup"><span data-stu-id="7d125-128">The following table shows the properties that are required when you create the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>

|<span data-ttu-id="7d125-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d125-129">Property</span></span>|<span data-ttu-id="7d125-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d125-130">Type</span></span>|<span data-ttu-id="7d125-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d125-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d125-132">id</span><span class="sxs-lookup"><span data-stu-id="7d125-132">id</span></span>|<span data-ttu-id="7d125-133">String</span><span class="sxs-lookup"><span data-stu-id="7d125-133">String</span></span>|<span data-ttu-id="7d125-134">A ID da categoria</span><span class="sxs-lookup"><span data-stu-id="7d125-134">The category ID</span></span>|
|<span data-ttu-id="7d125-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7d125-135">displayName</span></span>|<span data-ttu-id="7d125-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d125-136">String</span></span>|<span data-ttu-id="7d125-137">O nome da categoria</span><span class="sxs-lookup"><span data-stu-id="7d125-137">The category name</span></span>|
|<span data-ttu-id="7d125-138">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="7d125-138">hasRequiredSetting</span></span>|<span data-ttu-id="7d125-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d125-139">Boolean</span></span>|<span data-ttu-id="7d125-140">A categoria contém a configuração necessária de nível superior</span><span class="sxs-lookup"><span data-stu-id="7d125-140">The category contains top level required setting</span></span>|



## <a name="response"></a><span data-ttu-id="7d125-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d125-141">Response</span></span>
<span data-ttu-id="7d125-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d125-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d125-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d125-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d125-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d125-144">Request</span></span>
<span data-ttu-id="7d125-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d125-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d125-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d125-146">Response</span></span>
<span data-ttu-id="7d125-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d125-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






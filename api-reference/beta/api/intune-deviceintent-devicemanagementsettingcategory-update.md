---
title: Atualizar deviceManagementSettingCategory
description: Atualize as propriedades de um objeto deviceManagementSettingCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b98199e9e5f691cbceead1b22657bb31c2fb6b6c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136633"
---
# <a name="update-devicemanagementsettingcategory"></a><span data-ttu-id="efe93-103">Atualizar deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="efe93-103">Update deviceManagementSettingCategory</span></span>

<span data-ttu-id="efe93-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efe93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efe93-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="efe93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efe93-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="efe93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efe93-107">Atualize as propriedades de [um objeto deviceManagementSettingCategory.](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="efe93-107">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efe93-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="efe93-108">Prerequisites</span></span>
<span data-ttu-id="efe93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efe93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efe93-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efe93-111">Permission type</span></span>|<span data-ttu-id="efe93-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="efe93-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efe93-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efe93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efe93-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe93-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="efe93-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efe93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efe93-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efe93-116">Not supported.</span></span>|
|<span data-ttu-id="efe93-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efe93-117">Application</span></span>|<span data-ttu-id="efe93-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe93-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efe93-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efe93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="efe93-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efe93-120">Request headers</span></span>
|<span data-ttu-id="efe93-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="efe93-121">Header</span></span>|<span data-ttu-id="efe93-122">Valor</span><span class="sxs-lookup"><span data-stu-id="efe93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efe93-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="efe93-123">Authorization</span></span>|<span data-ttu-id="efe93-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efe93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efe93-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="efe93-125">Accept</span></span>|<span data-ttu-id="efe93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efe93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efe93-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efe93-127">Request body</span></span>
<span data-ttu-id="efe93-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementSettingCategory.](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="efe93-128">In the request body, supply a JSON representation for the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

<span data-ttu-id="efe93-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span><span class="sxs-lookup"><span data-stu-id="efe93-129">The following table shows the properties that are required when you create the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>

|<span data-ttu-id="efe93-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efe93-130">Property</span></span>|<span data-ttu-id="efe93-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="efe93-131">Type</span></span>|<span data-ttu-id="efe93-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="efe93-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efe93-133">id</span><span class="sxs-lookup"><span data-stu-id="efe93-133">id</span></span>|<span data-ttu-id="efe93-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efe93-134">String</span></span>|<span data-ttu-id="efe93-135">A ID da categoria</span><span class="sxs-lookup"><span data-stu-id="efe93-135">The category ID</span></span>|
|<span data-ttu-id="efe93-136">displayName</span><span class="sxs-lookup"><span data-stu-id="efe93-136">displayName</span></span>|<span data-ttu-id="efe93-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efe93-137">String</span></span>|<span data-ttu-id="efe93-138">O nome da categoria</span><span class="sxs-lookup"><span data-stu-id="efe93-138">The category name</span></span>|
|<span data-ttu-id="efe93-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="efe93-139">hasRequiredSetting</span></span>|<span data-ttu-id="efe93-140">Booleano</span><span class="sxs-lookup"><span data-stu-id="efe93-140">Boolean</span></span>|<span data-ttu-id="efe93-141">A categoria contém a configuração necessária de nível superior</span><span class="sxs-lookup"><span data-stu-id="efe93-141">The category contains top level required setting</span></span>|



## <a name="response"></a><span data-ttu-id="efe93-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="efe93-142">Response</span></span>
<span data-ttu-id="efe93-143">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efe93-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efe93-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efe93-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="efe93-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efe93-145">Request</span></span>
<span data-ttu-id="efe93-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efe93-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="efe93-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="efe93-147">Response</span></span>
<span data-ttu-id="efe93-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efe93-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





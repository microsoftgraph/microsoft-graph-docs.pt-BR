---
title: Criar deviceManagementSettingCategory
description: Criar um novo objeto deviceManagementSettingCategory.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 52fe09f9c5ebd74c6d665f990836d1e0006a3c7b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381614"
---
# <a name="create-devicemanagementsettingcategory"></a><span data-ttu-id="19ebd-103">Criar deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="19ebd-103">Create deviceManagementSettingCategory</span></span>

<span data-ttu-id="19ebd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19ebd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19ebd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="19ebd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19ebd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="19ebd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19ebd-107">Criar um novo objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="19ebd-107">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19ebd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="19ebd-108">Prerequisites</span></span>
<span data-ttu-id="19ebd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19ebd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19ebd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19ebd-111">Permission type</span></span>|<span data-ttu-id="19ebd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="19ebd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19ebd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19ebd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19ebd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19ebd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19ebd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19ebd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19ebd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19ebd-116">Not supported.</span></span>|
|<span data-ttu-id="19ebd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19ebd-117">Application</span></span>|<span data-ttu-id="19ebd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19ebd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19ebd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19ebd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/categories
```

## <a name="request-headers"></a><span data-ttu-id="19ebd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19ebd-120">Request headers</span></span>
|<span data-ttu-id="19ebd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19ebd-121">Header</span></span>|<span data-ttu-id="19ebd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="19ebd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19ebd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="19ebd-123">Authorization</span></span>|<span data-ttu-id="19ebd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19ebd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19ebd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="19ebd-125">Accept</span></span>|<span data-ttu-id="19ebd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19ebd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19ebd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19ebd-127">Request body</span></span>
<span data-ttu-id="19ebd-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="19ebd-128">In the request body, supply a JSON representation for the deviceManagementSettingCategory object.</span></span>

<span data-ttu-id="19ebd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="19ebd-129">The following table shows the properties that are required when you create the deviceManagementSettingCategory.</span></span>

|<span data-ttu-id="19ebd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19ebd-130">Property</span></span>|<span data-ttu-id="19ebd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="19ebd-131">Type</span></span>|<span data-ttu-id="19ebd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="19ebd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19ebd-133">id</span><span class="sxs-lookup"><span data-stu-id="19ebd-133">id</span></span>|<span data-ttu-id="19ebd-134">String</span><span class="sxs-lookup"><span data-stu-id="19ebd-134">String</span></span>|<span data-ttu-id="19ebd-135">A ID da categoria</span><span class="sxs-lookup"><span data-stu-id="19ebd-135">The category ID</span></span>|
|<span data-ttu-id="19ebd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="19ebd-136">displayName</span></span>|<span data-ttu-id="19ebd-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19ebd-137">String</span></span>|<span data-ttu-id="19ebd-138">O nome da categoria</span><span class="sxs-lookup"><span data-stu-id="19ebd-138">The category name</span></span>|
|<span data-ttu-id="19ebd-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="19ebd-139">hasRequiredSetting</span></span>|<span data-ttu-id="19ebd-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="19ebd-140">Boolean</span></span>|<span data-ttu-id="19ebd-141">A categoria contém a configuração necessária de nível superior</span><span class="sxs-lookup"><span data-stu-id="19ebd-141">The category contains top level required setting</span></span>|



## <a name="response"></a><span data-ttu-id="19ebd-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="19ebd-142">Response</span></span>
<span data-ttu-id="19ebd-143">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19ebd-143">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19ebd-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19ebd-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="19ebd-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19ebd-145">Request</span></span>
<span data-ttu-id="19ebd-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19ebd-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/categories
Content-type: application/json
Content-length: 144

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="19ebd-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="19ebd-147">Response</span></span>
<span data-ttu-id="19ebd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19ebd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 193

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```




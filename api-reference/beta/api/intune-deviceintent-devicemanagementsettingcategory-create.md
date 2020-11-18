---
title: Criar deviceManagementSettingCategory
description: Criar um novo objeto deviceManagementSettingCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c889962597896fefc5a2be03a44bc4121d5a7fb5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49203576"
---
# <a name="create-devicemanagementsettingcategory"></a><span data-ttu-id="5d8c3-103">Criar deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="5d8c3-103">Create deviceManagementSettingCategory</span></span>

<span data-ttu-id="5d8c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d8c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d8c3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d8c3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d8c3-107">Criar um novo objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="5d8c3-107">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d8c3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5d8c3-108">Prerequisites</span></span>
<span data-ttu-id="5d8c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d8c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d8c3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d8c3-111">Permission type</span></span>|<span data-ttu-id="5d8c3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5d8c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d8c3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d8c3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d8c3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d8c3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5d8c3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d8c3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d8c3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-116">Not supported.</span></span>|
|<span data-ttu-id="5d8c3-117">Application</span><span class="sxs-lookup"><span data-stu-id="5d8c3-117">Application</span></span>|<span data-ttu-id="5d8c3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d8c3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d8c3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d8c3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/categories
```

## <a name="request-headers"></a><span data-ttu-id="5d8c3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d8c3-120">Request headers</span></span>
|<span data-ttu-id="5d8c3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5d8c3-121">Header</span></span>|<span data-ttu-id="5d8c3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5d8c3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d8c3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d8c3-123">Authorization</span></span>|<span data-ttu-id="5d8c3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d8c3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5d8c3-125">Accept</span></span>|<span data-ttu-id="5d8c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d8c3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d8c3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d8c3-127">Request body</span></span>
<span data-ttu-id="5d8c3-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-128">In the request body, supply a JSON representation for the deviceManagementSettingCategory object.</span></span>

<span data-ttu-id="5d8c3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-129">The following table shows the properties that are required when you create the deviceManagementSettingCategory.</span></span>

|<span data-ttu-id="5d8c3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d8c3-130">Property</span></span>|<span data-ttu-id="5d8c3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d8c3-131">Type</span></span>|<span data-ttu-id="5d8c3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d8c3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d8c3-133">id</span><span class="sxs-lookup"><span data-stu-id="5d8c3-133">id</span></span>|<span data-ttu-id="5d8c3-134">String</span><span class="sxs-lookup"><span data-stu-id="5d8c3-134">String</span></span>|<span data-ttu-id="5d8c3-135">A ID da categoria</span><span class="sxs-lookup"><span data-stu-id="5d8c3-135">The category ID</span></span>|
|<span data-ttu-id="5d8c3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5d8c3-136">displayName</span></span>|<span data-ttu-id="5d8c3-137">String</span><span class="sxs-lookup"><span data-stu-id="5d8c3-137">String</span></span>|<span data-ttu-id="5d8c3-138">O nome da categoria</span><span class="sxs-lookup"><span data-stu-id="5d8c3-138">The category name</span></span>|
|<span data-ttu-id="5d8c3-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="5d8c3-139">hasRequiredSetting</span></span>|<span data-ttu-id="5d8c3-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="5d8c3-140">Boolean</span></span>|<span data-ttu-id="5d8c3-141">A categoria contém a configuração necessária de nível superior</span><span class="sxs-lookup"><span data-stu-id="5d8c3-141">The category contains top level required setting</span></span>|



## <a name="response"></a><span data-ttu-id="5d8c3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d8c3-142">Response</span></span>
<span data-ttu-id="5d8c3-143">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-143">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d8c3-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d8c3-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d8c3-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d8c3-145">Request</span></span>
<span data-ttu-id="5d8c3-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5d8c3-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d8c3-147">Response</span></span>
<span data-ttu-id="5d8c3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d8c3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





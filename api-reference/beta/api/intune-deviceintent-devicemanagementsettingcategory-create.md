---
title: Criar deviceManagementSettingCategory
description: Criar um novo objeto deviceManagementSettingCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c30f01bfbfd82fd4fc4dca73055c1cf3a490fba
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33915687"
---
# <a name="create-devicemanagementsettingcategory"></a><span data-ttu-id="8325d-103">Criar deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="8325d-103">Create deviceManagementSettingCategory</span></span>

> <span data-ttu-id="8325d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8325d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8325d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8325d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8325d-106">Criar um novo objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="8325d-106">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8325d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8325d-107">Prerequisites</span></span>
<span data-ttu-id="8325d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8325d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8325d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8325d-110">Permission type</span></span>|<span data-ttu-id="8325d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8325d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8325d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8325d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8325d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8325d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8325d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8325d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8325d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8325d-115">Not supported.</span></span>|
|<span data-ttu-id="8325d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8325d-116">Application</span></span>|<span data-ttu-id="8325d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8325d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8325d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8325d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/categories
```

## <a name="request-headers"></a><span data-ttu-id="8325d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8325d-119">Request headers</span></span>
|<span data-ttu-id="8325d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8325d-120">Header</span></span>|<span data-ttu-id="8325d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8325d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8325d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8325d-122">Authorization</span></span>|<span data-ttu-id="8325d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8325d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8325d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8325d-124">Accept</span></span>|<span data-ttu-id="8325d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8325d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8325d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8325d-126">Request body</span></span>
<span data-ttu-id="8325d-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="8325d-127">In the request body, supply a JSON representation for the deviceManagementSettingCategory object.</span></span>

<span data-ttu-id="8325d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="8325d-128">The following table shows the properties that are required when you create the deviceManagementSettingCategory.</span></span>

|<span data-ttu-id="8325d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8325d-129">Property</span></span>|<span data-ttu-id="8325d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8325d-130">Type</span></span>|<span data-ttu-id="8325d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8325d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8325d-132">id</span><span class="sxs-lookup"><span data-stu-id="8325d-132">id</span></span>|<span data-ttu-id="8325d-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8325d-133">String</span></span>|<span data-ttu-id="8325d-134">A ID da categoria</span><span class="sxs-lookup"><span data-stu-id="8325d-134">The category ID</span></span>|
|<span data-ttu-id="8325d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8325d-135">displayName</span></span>|<span data-ttu-id="8325d-136">String</span><span class="sxs-lookup"><span data-stu-id="8325d-136">String</span></span>|<span data-ttu-id="8325d-137">O nome da categoria</span><span class="sxs-lookup"><span data-stu-id="8325d-137">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="8325d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8325d-138">Response</span></span>
<span data-ttu-id="8325d-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8325d-139">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8325d-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8325d-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="8325d-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8325d-141">Request</span></span>
<span data-ttu-id="8325d-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8325d-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/categories
Content-type: application/json
Content-length: 113

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="8325d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="8325d-143">Response</span></span>
<span data-ttu-id="8325d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8325d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 162

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
  "displayName": "Display Name value"
}
```





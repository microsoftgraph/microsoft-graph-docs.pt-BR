---
title: Atualizar deviceManagementTemplateSettingCategory
description: Atualiza as propriedades de um objeto deviceManagementTemplateSettingCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca7fe9ee187e464c1b88d8ef989c157b1b066dc9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33914587"
---
# <a name="update-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="0c5f1-103">Atualizar deviceManagementTemplateSettingCategory</span><span class="sxs-lookup"><span data-stu-id="0c5f1-103">Update deviceManagementTemplateSettingCategory</span></span>

> <span data-ttu-id="0c5f1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0c5f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c5f1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c5f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c5f1-106">Atualiza as propriedades de um objeto [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="0c5f1-106">Update the properties of a [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c5f1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c5f1-107">Prerequisites</span></span>
<span data-ttu-id="0c5f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c5f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c5f1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c5f1-110">Permission type</span></span>|<span data-ttu-id="0c5f1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c5f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c5f1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c5f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c5f1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c5f1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c5f1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c5f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c5f1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c5f1-115">Not supported.</span></span>|
|<span data-ttu-id="0c5f1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c5f1-116">Application</span></span>|<span data-ttu-id="0c5f1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c5f1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c5f1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c5f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="0c5f1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c5f1-119">Request headers</span></span>
|<span data-ttu-id="0c5f1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c5f1-120">Header</span></span>|<span data-ttu-id="0c5f1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0c5f1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c5f1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c5f1-122">Authorization</span></span>|<span data-ttu-id="0c5f1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c5f1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c5f1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c5f1-124">Accept</span></span>|<span data-ttu-id="0c5f1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c5f1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c5f1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c5f1-126">Request body</span></span>
<span data-ttu-id="0c5f1-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="0c5f1-127">In the request body, supply a JSON representation for the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

<span data-ttu-id="0c5f1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md).</span><span class="sxs-lookup"><span data-stu-id="0c5f1-128">The following table shows the properties that are required when you create the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md).</span></span>

|<span data-ttu-id="0c5f1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c5f1-129">Property</span></span>|<span data-ttu-id="0c5f1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c5f1-130">Type</span></span>|<span data-ttu-id="0c5f1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c5f1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c5f1-132">id</span><span class="sxs-lookup"><span data-stu-id="0c5f1-132">id</span></span>|<span data-ttu-id="0c5f1-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c5f1-133">String</span></span>|<span data-ttu-id="0c5f1-134">A ID de categoria herdada de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="0c5f1-134">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="0c5f1-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0c5f1-135">displayName</span></span>|<span data-ttu-id="0c5f1-136">String</span><span class="sxs-lookup"><span data-stu-id="0c5f1-136">String</span></span>|<span data-ttu-id="0c5f1-137">O nome da categoria herdado de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="0c5f1-137">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0c5f1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c5f1-138">Response</span></span>
<span data-ttu-id="0c5f1-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c5f1-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c5f1-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c5f1-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c5f1-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c5f1-141">Request</span></span>
<span data-ttu-id="0c5f1-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c5f1-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
Content-type: application/json
Content-length: 121

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="0c5f1-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c5f1-143">Response</span></span>
<span data-ttu-id="0c5f1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c5f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 170

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "id": "cd213562-3562-cd21-6235-21cd623521cd",
  "displayName": "Display Name value"
}
```





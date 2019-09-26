---
title: Listar deviceManagementSettingCategories
description: Listar Propriedades e relações dos objetos deviceManagementSettingCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1eda53c2fce21e52743c300abec2cf5463bdebd
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37189246"
---
# <a name="list-devicemanagementsettingcategories"></a><span data-ttu-id="63442-103">Listar deviceManagementSettingCategories</span><span class="sxs-lookup"><span data-stu-id="63442-103">List deviceManagementSettingCategories</span></span>

> <span data-ttu-id="63442-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63442-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63442-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63442-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63442-106">Listar Propriedades e relações dos objetos [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="63442-106">List properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63442-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63442-107">Prerequisites</span></span>
<span data-ttu-id="63442-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63442-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63442-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63442-110">Permission type</span></span>|<span data-ttu-id="63442-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63442-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63442-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63442-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63442-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63442-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="63442-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63442-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63442-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63442-115">Not supported.</span></span>|
|<span data-ttu-id="63442-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63442-116">Application</span></span>|<span data-ttu-id="63442-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63442-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63442-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63442-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/categories
```

## <a name="request-headers"></a><span data-ttu-id="63442-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63442-119">Request headers</span></span>
|<span data-ttu-id="63442-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63442-120">Header</span></span>|<span data-ttu-id="63442-121">Valor</span><span class="sxs-lookup"><span data-stu-id="63442-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63442-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="63442-122">Authorization</span></span>|<span data-ttu-id="63442-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63442-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63442-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63442-124">Accept</span></span>|<span data-ttu-id="63442-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63442-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63442-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63442-126">Request body</span></span>
<span data-ttu-id="63442-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63442-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63442-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="63442-128">Response</span></span>
<span data-ttu-id="63442-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63442-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63442-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63442-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="63442-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63442-131">Request</span></span>
<span data-ttu-id="63442-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63442-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/categories
```

### <a name="response"></a><span data-ttu-id="63442-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="63442-133">Response</span></span>
<span data-ttu-id="63442-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63442-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 207

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
      "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
      "displayName": "Display Name value"
    }
  ]
}
```





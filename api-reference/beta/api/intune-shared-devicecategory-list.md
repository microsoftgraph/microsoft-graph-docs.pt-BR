---
title: Listar deviceCategories
description: Lista propriedades e relações dos objetos deviceCategory.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d5086dd832d3228e7317bd0cd4760635ce2d637b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801226"
---
# <a name="list-devicecategories"></a><span data-ttu-id="ad77e-103">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="ad77e-103">List deviceCategories</span></span>

> <span data-ttu-id="ad77e-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ad77e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ad77e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ad77e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad77e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ad77e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad77e-107">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="ad77e-107">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad77e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ad77e-108">Prerequisites</span></span>
<span data-ttu-id="ad77e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad77e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad77e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad77e-111">Permission type</span></span>|<span data-ttu-id="ad77e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ad77e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad77e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad77e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ad77e-114">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="ad77e-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ad77e-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad77e-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ad77e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad77e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad77e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad77e-117">Not supported.</span></span>|
|<span data-ttu-id="ad77e-118">Application</span><span class="sxs-lookup"><span data-stu-id="ad77e-118">Application</span></span>||
| <span data-ttu-id="ad77e-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="ad77e-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ad77e-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad77e-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad77e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad77e-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="ad77e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad77e-122">Request headers</span></span>

|<span data-ttu-id="ad77e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad77e-123">Header</span></span>|<span data-ttu-id="ad77e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ad77e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad77e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad77e-125">Authorization</span></span>|<span data-ttu-id="ad77e-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad77e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad77e-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ad77e-127">Accept</span></span>|<span data-ttu-id="ad77e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ad77e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad77e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad77e-129">Request body</span></span>

<span data-ttu-id="ad77e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ad77e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad77e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad77e-131">Response</span></span>

<span data-ttu-id="ad77e-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad77e-132">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad77e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad77e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad77e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad77e-134">Request</span></span>

<span data-ttu-id="ad77e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad77e-135">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="ad77e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad77e-136">Response</span></span>

<span data-ttu-id="ad77e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad77e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCategory",
      "id": "f881b841-b841-f881-41b8-81f841b881f8",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```











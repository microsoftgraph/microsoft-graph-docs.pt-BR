---
title: Listar deviceCategories
description: Lista propriedades e relações dos objetos deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc7b4286d967274eafeafa3797d2fa57633f52e7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458879"
---
# <a name="list-devicecategories"></a><span data-ttu-id="52d58-103">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="52d58-103">List deviceCategories</span></span>

<span data-ttu-id="52d58-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="52d58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52d58-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="52d58-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="52d58-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="52d58-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52d58-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52d58-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52d58-108">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="52d58-108">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="52d58-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52d58-109">Prerequisites</span></span>
<span data-ttu-id="52d58-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52d58-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52d58-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52d58-112">Permission type</span></span>|<span data-ttu-id="52d58-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52d58-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52d58-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52d58-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="52d58-115">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="52d58-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="52d58-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="52d58-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="52d58-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52d58-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52d58-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52d58-118">Not supported.</span></span>|
|<span data-ttu-id="52d58-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52d58-119">Application</span></span>||
| <span data-ttu-id="52d58-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="52d58-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="52d58-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="52d58-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52d58-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52d58-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="52d58-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52d58-123">Request headers</span></span>

|<span data-ttu-id="52d58-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52d58-124">Header</span></span>|<span data-ttu-id="52d58-125">Valor</span><span class="sxs-lookup"><span data-stu-id="52d58-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52d58-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="52d58-126">Authorization</span></span>|<span data-ttu-id="52d58-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52d58-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52d58-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52d58-128">Accept</span></span>|<span data-ttu-id="52d58-129">application/json</span><span class="sxs-lookup"><span data-stu-id="52d58-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52d58-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52d58-130">Request body</span></span>

<span data-ttu-id="52d58-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52d58-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52d58-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="52d58-132">Response</span></span>

<span data-ttu-id="52d58-133">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52d58-133">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52d58-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52d58-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="52d58-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52d58-135">Request</span></span>

<span data-ttu-id="52d58-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52d58-136">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="52d58-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="52d58-137">Response</span></span>

<span data-ttu-id="52d58-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52d58-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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












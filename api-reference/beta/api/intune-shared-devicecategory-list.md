---
title: Listar deviceCategories
description: Lista propriedades e relações dos objetos deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ae7e210dff4e0aeb8d6c5806b1b63ec06eb55eb9
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196067"
---
# <a name="list-devicecategories"></a><span data-ttu-id="da759-103">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="da759-103">List deviceCategories</span></span>

> <span data-ttu-id="da759-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="da759-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="da759-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="da759-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da759-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da759-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da759-107">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="da759-107">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da759-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="da759-108">Prerequisites</span></span>
<span data-ttu-id="da759-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da759-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da759-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da759-111">Permission type</span></span>|<span data-ttu-id="da759-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da759-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da759-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da759-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="da759-114">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="da759-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="da759-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="da759-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="da759-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da759-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da759-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da759-117">Not supported.</span></span>|
|<span data-ttu-id="da759-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da759-118">Application</span></span>||
| <span data-ttu-id="da759-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="da759-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="da759-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="da759-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da759-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da759-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="da759-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da759-122">Request headers</span></span>

|<span data-ttu-id="da759-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da759-123">Header</span></span>|<span data-ttu-id="da759-124">Valor</span><span class="sxs-lookup"><span data-stu-id="da759-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da759-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="da759-125">Authorization</span></span>|<span data-ttu-id="da759-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da759-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da759-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="da759-127">Accept</span></span>|<span data-ttu-id="da759-128">application/json</span><span class="sxs-lookup"><span data-stu-id="da759-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da759-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da759-129">Request body</span></span>

<span data-ttu-id="da759-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da759-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da759-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="da759-131">Response</span></span>

<span data-ttu-id="da759-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da759-132">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da759-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da759-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="da759-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da759-134">Request</span></span>

<span data-ttu-id="da759-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da759-135">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="da759-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="da759-136">Response</span></span>

<span data-ttu-id="da759-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da759-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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








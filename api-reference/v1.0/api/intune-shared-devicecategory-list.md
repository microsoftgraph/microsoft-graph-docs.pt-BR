---
title: Listar deviceCategories
description: Lista propriedades e relações dos objetos deviceCategory.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6463f41b2e9045065e2f783f80428a94d3944f9c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512087"
---
# <a name="list-devicecategories"></a><span data-ttu-id="292ae-103">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="292ae-103">List deviceCategories</span></span>

<span data-ttu-id="292ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="292ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="292ae-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="292ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="292ae-106">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="292ae-106">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="292ae-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="292ae-107">Prerequisites</span></span>
<span data-ttu-id="292ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="292ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="292ae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="292ae-110">Permission type</span></span>|<span data-ttu-id="292ae-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="292ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="292ae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="292ae-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="292ae-113">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="292ae-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="292ae-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="292ae-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="292ae-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="292ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="292ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="292ae-116">Not supported.</span></span>|
|<span data-ttu-id="292ae-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="292ae-117">Application</span></span>|<span data-ttu-id="292ae-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="292ae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="292ae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="292ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="292ae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="292ae-120">Request headers</span></span>
|<span data-ttu-id="292ae-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="292ae-121">Header</span></span>|<span data-ttu-id="292ae-122">Valor</span><span class="sxs-lookup"><span data-stu-id="292ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="292ae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="292ae-123">Authorization</span></span>|<span data-ttu-id="292ae-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="292ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="292ae-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="292ae-125">Accept</span></span>|<span data-ttu-id="292ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="292ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="292ae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="292ae-127">Request body</span></span>
<span data-ttu-id="292ae-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="292ae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="292ae-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="292ae-129">Response</span></span>
<span data-ttu-id="292ae-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="292ae-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="292ae-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="292ae-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="292ae-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="292ae-132">Request</span></span>
<span data-ttu-id="292ae-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="292ae-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="292ae-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="292ae-134">Response</span></span>
<span data-ttu-id="292ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="292ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





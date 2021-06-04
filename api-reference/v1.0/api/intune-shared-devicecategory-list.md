---
title: Listar deviceCategories
description: Lista propriedades e relações dos objetos deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 65d69d7602c66a18edc0f4cf50d52a39aeefd2a0
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732206"
---
# <a name="list-devicecategories"></a><span data-ttu-id="9d119-103">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="9d119-103">List deviceCategories</span></span>

<span data-ttu-id="9d119-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d119-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d119-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d119-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d119-106">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="9d119-106">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d119-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9d119-107">Prerequisites</span></span>
<span data-ttu-id="9d119-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d119-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d119-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d119-110">Permission type</span></span>|<span data-ttu-id="9d119-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9d119-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d119-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d119-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9d119-113">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="9d119-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="9d119-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d119-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9d119-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d119-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d119-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d119-116">Not supported.</span></span>|
|<span data-ttu-id="9d119-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d119-117">Application</span></span>|<span data-ttu-id="9d119-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d119-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d119-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d119-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="9d119-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d119-120">Request headers</span></span>
|<span data-ttu-id="9d119-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9d119-121">Header</span></span>|<span data-ttu-id="9d119-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9d119-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d119-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d119-123">Authorization</span></span>|<span data-ttu-id="9d119-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d119-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d119-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9d119-125">Accept</span></span>|<span data-ttu-id="9d119-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d119-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d119-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d119-127">Request body</span></span>
<span data-ttu-id="9d119-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9d119-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d119-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d119-129">Response</span></span>
<span data-ttu-id="9d119-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d119-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d119-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d119-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d119-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d119-132">Request</span></span>
<span data-ttu-id="9d119-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d119-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="9d119-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d119-134">Response</span></span>
<span data-ttu-id="9d119-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d119-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










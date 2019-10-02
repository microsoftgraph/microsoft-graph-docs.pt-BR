---
title: Listar deviceCategories
description: Lista propriedades e relações dos objetos deviceCategory.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 780cb239119d28941a1cfaf73d28bc8749120873
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361494"
---
# <a name="list-devicecategories"></a><span data-ttu-id="b5942-103">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="b5942-103">List deviceCategories</span></span>

> <span data-ttu-id="b5942-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b5942-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5942-105">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b5942-105">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5942-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b5942-106">Prerequisites</span></span>
<span data-ttu-id="b5942-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5942-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5942-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5942-109">Permission type</span></span>|<span data-ttu-id="b5942-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b5942-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5942-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5942-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b5942-112">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="b5942-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b5942-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5942-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b5942-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5942-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5942-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5942-115">Not supported.</span></span>|
|<span data-ttu-id="b5942-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5942-116">Application</span></span>|<span data-ttu-id="b5942-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5942-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5942-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5942-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="b5942-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5942-119">Request headers</span></span>
|<span data-ttu-id="b5942-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b5942-120">Header</span></span>|<span data-ttu-id="b5942-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b5942-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5942-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5942-122">Authorization</span></span>|<span data-ttu-id="b5942-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5942-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5942-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b5942-124">Accept</span></span>|<span data-ttu-id="b5942-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5942-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5942-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5942-126">Request body</span></span>
<span data-ttu-id="b5942-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b5942-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5942-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5942-128">Response</span></span>
<span data-ttu-id="b5942-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5942-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5942-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5942-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5942-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5942-131">Request</span></span>
<span data-ttu-id="b5942-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5942-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="b5942-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5942-133">Response</span></span>
<span data-ttu-id="b5942-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5942-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





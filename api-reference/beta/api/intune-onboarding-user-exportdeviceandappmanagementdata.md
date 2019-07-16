---
title: função exportDeviceAndAppManagementData
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9fd7b9ddcf82ce8ec65e2e58d97ea1a8b08f2ea7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741270"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="ba7de-103">função exportDeviceAndAppManagementData</span><span class="sxs-lookup"><span data-stu-id="ba7de-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="ba7de-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ba7de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba7de-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba7de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba7de-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ba7de-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba7de-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba7de-107">Prerequisites</span></span>
<span data-ttu-id="ba7de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba7de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba7de-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba7de-110">Permission type</span></span>|<span data-ttu-id="ba7de-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ba7de-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba7de-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba7de-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba7de-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba7de-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ba7de-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba7de-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba7de-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba7de-115">Not supported.</span></span>|
|<span data-ttu-id="ba7de-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba7de-116">Application</span></span>|<span data-ttu-id="ba7de-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba7de-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba7de-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba7de-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="ba7de-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba7de-119">Request headers</span></span>
|<span data-ttu-id="ba7de-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba7de-120">Header</span></span>|<span data-ttu-id="ba7de-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ba7de-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba7de-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba7de-122">Authorization</span></span>|<span data-ttu-id="ba7de-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba7de-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba7de-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba7de-124">Accept</span></span>|<span data-ttu-id="ba7de-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba7de-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba7de-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba7de-126">Request body</span></span>
<span data-ttu-id="ba7de-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="ba7de-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ba7de-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="ba7de-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ba7de-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba7de-129">Property</span></span>|<span data-ttu-id="ba7de-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba7de-130">Type</span></span>|<span data-ttu-id="ba7de-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba7de-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba7de-132">skip</span><span class="sxs-lookup"><span data-stu-id="ba7de-132">skip</span></span>|<span data-ttu-id="ba7de-133">Int32</span><span class="sxs-lookup"><span data-stu-id="ba7de-133">Int32</span></span>|<span data-ttu-id="ba7de-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ba7de-134">Not yet documented</span></span>|
|<span data-ttu-id="ba7de-135">top</span><span class="sxs-lookup"><span data-stu-id="ba7de-135">top</span></span>|<span data-ttu-id="ba7de-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ba7de-136">Int32</span></span>|<span data-ttu-id="ba7de-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ba7de-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ba7de-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba7de-138">Response</span></span>
<span data-ttu-id="ba7de-139">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba7de-139">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba7de-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba7de-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba7de-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba7de-141">Request</span></span>
<span data-ttu-id="ba7de-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba7de-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="ba7de-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba7de-143">Response</span></span>
<span data-ttu-id="ba7de-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba7de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 143

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementData",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```






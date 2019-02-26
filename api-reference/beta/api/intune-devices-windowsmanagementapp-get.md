---
title: Obter windowsManagementApp
description: Leia as propriedades e as relações do objeto windowsManagementApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37a99e0d318ec6bee73591d5882af6ffff6503fa
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161345"
---
# <a name="get-windowsmanagementapp"></a><span data-ttu-id="c098b-103">Obter windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="c098b-103">Get windowsManagementApp</span></span>

> <span data-ttu-id="c098b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c098b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c098b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c098b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c098b-106">Leia as propriedades e as relações do objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="c098b-106">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c098b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c098b-107">Prerequisites</span></span>
<span data-ttu-id="c098b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c098b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c098b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c098b-110">Permission type</span></span>|<span data-ttu-id="c098b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c098b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c098b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c098b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c098b-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c098b-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c098b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c098b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c098b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c098b-115">Not supported.</span></span>|
|<span data-ttu-id="c098b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c098b-116">Application</span></span>|<span data-ttu-id="c098b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c098b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c098b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c098b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c098b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c098b-119">Optional query parameters</span></span>
<span data-ttu-id="c098b-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c098b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c098b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c098b-121">Request headers</span></span>
|<span data-ttu-id="c098b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c098b-122">Header</span></span>|<span data-ttu-id="c098b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c098b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c098b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c098b-124">Authorization</span></span>|<span data-ttu-id="c098b-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c098b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c098b-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c098b-126">Accept</span></span>|<span data-ttu-id="c098b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c098b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c098b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c098b-128">Request body</span></span>
<span data-ttu-id="c098b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c098b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c098b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c098b-130">Response</span></span>
<span data-ttu-id="c098b-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c098b-131">If successful, this method returns a `200 OK` response code and [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c098b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c098b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c098b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c098b-133">Request</span></span>
<span data-ttu-id="c098b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c098b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
```

### <a name="response"></a><span data-ttu-id="c098b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c098b-135">Response</span></span>
<span data-ttu-id="c098b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c098b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsManagementApp",
    "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
    "availableVersion": "Available Version value"
  }
}
```





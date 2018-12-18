---
title: Obter deviceCategory
description: Ler propriedades de leitura e relações do objeto deviceCategory.
author: tfitzmac
ms.openlocfilehash: 4a43f0d2551e98ce0a51e28764c90b234015ec29
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331059"
---
# <a name="get-devicecategory"></a><span data-ttu-id="3fdd1-103">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="3fdd1-103">Get deviceCategory</span></span>

> <span data-ttu-id="3fdd1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3fdd1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3fdd1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3fdd1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3fdd1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3fdd1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3fdd1-107">Ler propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="3fdd1-107">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fdd1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3fdd1-108">Prerequisites</span></span>

<span data-ttu-id="3fdd1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fdd1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fdd1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3fdd1-111">Permission type</span></span>|<span data-ttu-id="3fdd1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3fdd1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fdd1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fdd1-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3fdd1-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="3fdd1-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="3fdd1-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fdd1-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="3fdd1-116">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="3fdd1-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="3fdd1-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fdd1-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3fdd1-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fdd1-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fdd1-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fdd1-119">Not supported.</span></span>|
|<span data-ttu-id="3fdd1-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3fdd1-120">Application</span></span>|<span data-ttu-id="3fdd1-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fdd1-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fdd1-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fdd1-122">HTTP Request</span></span>

<span data-ttu-id="3fdd1-123">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="3fdd1-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

<span data-ttu-id="3fdd1-124">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="3fdd1-124">**Onboarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3fdd1-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3fdd1-125">Optional query parameters</span></span>

<span data-ttu-id="3fdd1-126">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3fdd1-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3fdd1-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3fdd1-127">Request headers</span></span>

|<span data-ttu-id="3fdd1-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3fdd1-128">Header</span></span>|<span data-ttu-id="3fdd1-129">Valor</span><span class="sxs-lookup"><span data-stu-id="3fdd1-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fdd1-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="3fdd1-130">Authorization</span></span>|<span data-ttu-id="3fdd1-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fdd1-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fdd1-132">Accept</span><span class="sxs-lookup"><span data-stu-id="3fdd1-132">Accept</span></span>|<span data-ttu-id="3fdd1-133">application/json</span><span class="sxs-lookup"><span data-stu-id="3fdd1-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fdd1-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3fdd1-134">Request body</span></span>

<span data-ttu-id="3fdd1-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3fdd1-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fdd1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fdd1-136">Response</span></span>

<span data-ttu-id="3fdd1-137">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fdd1-137">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fdd1-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fdd1-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fdd1-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3fdd1-139">Request</span></span>

<span data-ttu-id="3fdd1-140">Eis aqui são exemplos da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fdd1-140">Here is are examples of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="3fdd1-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fdd1-141">Response</span></span>

<span data-ttu-id="3fdd1-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fdd1-142">Here is an example of the response.</span></span> <span data-ttu-id="3fdd1-143">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="3fdd1-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3fdd1-144">Propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="3fdd1-144">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 211

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCategory",
    "id": "f881b841-b841-f881-41b8-81f841b881f8",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```




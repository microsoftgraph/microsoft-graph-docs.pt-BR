---
title: Get detectedApp
description: Ler propriedades e relações do objeto detectedApp.
author: tfitzmac
ms.openlocfilehash: d8d52d614d060d433fcee468a0b5663de33a5dc6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311953"
---
# <a name="get-detectedapp"></a><span data-ttu-id="6e66e-103">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="6e66e-103">Get detectedApp</span></span>

> <span data-ttu-id="6e66e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6e66e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e66e-105">Ler propriedades e relações do objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="6e66e-105">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6e66e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e66e-106">Prerequisites</span></span>
<span data-ttu-id="6e66e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e66e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e66e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e66e-109">Permission type</span></span>|<span data-ttu-id="6e66e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e66e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e66e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e66e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6e66e-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e66e-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6e66e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e66e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e66e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e66e-114">Not supported.</span></span>|
|<span data-ttu-id="6e66e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e66e-115">Application</span></span>|<span data-ttu-id="6e66e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e66e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e66e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e66e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e66e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6e66e-118">Optional query parameters</span></span>
<span data-ttu-id="6e66e-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6e66e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6e66e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66e-120">Request headers</span></span>
|<span data-ttu-id="6e66e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e66e-121">Header</span></span>|<span data-ttu-id="6e66e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6e66e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e66e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e66e-123">Authorization</span></span>|<span data-ttu-id="6e66e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e66e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e66e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6e66e-125">Accept</span></span>|<span data-ttu-id="6e66e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e66e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e66e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66e-127">Request body</span></span>
<span data-ttu-id="6e66e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e66e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e66e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66e-129">Response</span></span>
<span data-ttu-id="6e66e-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [detectedApp](../resources/intune-devices-detectedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e66e-130">If successful, this method returns a `200 OK` response code and [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e66e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e66e-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6e66e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e66e-132">Request</span></span>
<span data-ttu-id="6e66e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e66e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}
```

### <a name="response"></a><span data-ttu-id="6e66e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e66e-134">Response</span></span>
<span data-ttu-id="6e66e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e66e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "value": {
    "@odata.type": "#microsoft.graph.detectedApp",
    "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
    "displayName": "Display Name value",
    "version": "Version value",
    "sizeInByte": 10,
    "deviceCount": 11
  }
}
```




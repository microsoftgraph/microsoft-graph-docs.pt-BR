---
title: Acessar managedDevice
description: Leia as propriedades e as relações do objeto managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fdcbb3cc8bd9aa34848768d83191ff42683a2b04
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160062"
---
# <a name="get-manageddevice"></a><span data-ttu-id="1c537-103">Acessar managedDevice</span><span class="sxs-lookup"><span data-stu-id="1c537-103">Get managedDevice</span></span>

<span data-ttu-id="1c537-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c537-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c537-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c537-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c537-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c537-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c537-107">Leia as propriedades e as relações do objeto [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1c537-107">Read properties and relationships of the [managedDevice](../resources/intune-shared-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c537-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c537-108">Prerequisites</span></span>
<span data-ttu-id="1c537-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c537-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c537-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c537-111">Permission type</span></span>|<span data-ttu-id="1c537-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c537-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c537-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c537-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c537-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c537-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1c537-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c537-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c537-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c537-116">Not supported.</span></span>|
|<span data-ttu-id="1c537-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c537-117">Application</span></span>|<span data-ttu-id="1c537-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c537-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c537-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c537-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices/{managedDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c537-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c537-120">Optional query parameters</span></span>
<span data-ttu-id="1c537-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c537-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c537-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c537-122">Request headers</span></span>
|<span data-ttu-id="1c537-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c537-123">Header</span></span>|<span data-ttu-id="1c537-124">Valor</span><span class="sxs-lookup"><span data-stu-id="1c537-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c537-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c537-125">Authorization</span></span>|<span data-ttu-id="1c537-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c537-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c537-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c537-127">Accept</span></span>|<span data-ttu-id="1c537-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1c537-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c537-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c537-129">Request body</span></span>
<span data-ttu-id="1c537-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c537-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c537-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c537-131">Response</span></span>
<span data-ttu-id="1c537-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedDevice](../resources/intune-shared-manageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c537-132">If successful, this method returns a `200 OK` response code and [managedDevice](../resources/intune-shared-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c537-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c537-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c537-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c537-134">Request</span></span>
<span data-ttu-id="1c537-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c537-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
```

### <a name="response"></a><span data-ttu-id="1c537-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c537-136">Response</span></span>
<span data-ttu-id="1c537-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c537-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 127

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDevice",
    "id": "705c034c-034c-705c-4c03-5c704c035c70"
  }
}
```





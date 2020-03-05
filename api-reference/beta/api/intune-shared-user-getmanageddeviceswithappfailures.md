---
title: função getManagedDevicesWithAppFailures
description: Recupera a lista de dispositivos com aplicativos com falha
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 17b56f1af0553255694c444d898ab85447846753
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458025"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="a34fc-103">função getManagedDevicesWithAppFailures</span><span class="sxs-lookup"><span data-stu-id="a34fc-103">getManagedDevicesWithAppFailures function</span></span>

<span data-ttu-id="a34fc-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a34fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a34fc-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a34fc-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a34fc-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a34fc-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a34fc-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a34fc-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a34fc-108">Recupera a lista de dispositivos com aplicativos com falha</span><span class="sxs-lookup"><span data-stu-id="a34fc-108">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a34fc-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a34fc-109">Prerequisites</span></span>
<span data-ttu-id="a34fc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a34fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a34fc-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a34fc-112">Permission type</span></span>|<span data-ttu-id="a34fc-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a34fc-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a34fc-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a34fc-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a34fc-115">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="a34fc-115">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="a34fc-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a34fc-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a34fc-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a34fc-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a34fc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a34fc-118">Not supported.</span></span>|
|<span data-ttu-id="a34fc-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a34fc-119">Application</span></span>||
| <span data-ttu-id="a34fc-120">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="a34fc-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="a34fc-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a34fc-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a34fc-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a34fc-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="a34fc-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a34fc-123">Request headers</span></span>
|<span data-ttu-id="a34fc-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a34fc-124">Header</span></span>|<span data-ttu-id="a34fc-125">Valor</span><span class="sxs-lookup"><span data-stu-id="a34fc-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a34fc-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="a34fc-126">Authorization</span></span>|<span data-ttu-id="a34fc-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a34fc-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a34fc-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a34fc-128">Accept</span></span>|<span data-ttu-id="a34fc-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a34fc-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a34fc-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a34fc-130">Request body</span></span>
<span data-ttu-id="a34fc-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a34fc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a34fc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a34fc-132">Response</span></span>
<span data-ttu-id="a34fc-133">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a34fc-133">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a34fc-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a34fc-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="a34fc-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a34fc-135">Request</span></span>
<span data-ttu-id="a34fc-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a34fc-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="a34fc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a34fc-137">Response</span></span>
<span data-ttu-id="a34fc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a34fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 74

{
  "value": [
    "Get Managed Devices With App Failures value"
  ]
}
```














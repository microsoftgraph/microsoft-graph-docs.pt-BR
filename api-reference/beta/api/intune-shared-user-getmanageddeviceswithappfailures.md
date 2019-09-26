---
title: função getManagedDevicesWithAppFailures
description: Recupera a lista de dispositivos com aplicativos com falha
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b20bf797b6e81ce78e75cee3d139b1e3de4dc3e
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195738"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="fc068-103">função getManagedDevicesWithAppFailures</span><span class="sxs-lookup"><span data-stu-id="fc068-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="fc068-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fc068-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fc068-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fc068-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc068-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc068-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc068-107">Recupera a lista de dispositivos com aplicativos com falha</span><span class="sxs-lookup"><span data-stu-id="fc068-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fc068-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fc068-108">Prerequisites</span></span>
<span data-ttu-id="fc068-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc068-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc068-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc068-111">Permission type</span></span>|<span data-ttu-id="fc068-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fc068-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc068-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc068-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fc068-114">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="fc068-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="fc068-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc068-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="fc068-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc068-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc068-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc068-117">Not supported.</span></span>|
|<span data-ttu-id="fc068-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc068-118">Application</span></span>||
| <span data-ttu-id="fc068-119">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="fc068-119">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="fc068-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc068-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc068-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc068-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="fc068-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc068-122">Request headers</span></span>
|<span data-ttu-id="fc068-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc068-123">Header</span></span>|<span data-ttu-id="fc068-124">Valor</span><span class="sxs-lookup"><span data-stu-id="fc068-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc068-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc068-125">Authorization</span></span>|<span data-ttu-id="fc068-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc068-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc068-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fc068-127">Accept</span></span>|<span data-ttu-id="fc068-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fc068-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc068-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc068-129">Request body</span></span>
<span data-ttu-id="fc068-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc068-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc068-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc068-131">Response</span></span>
<span data-ttu-id="fc068-132">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc068-132">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc068-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc068-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="fc068-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc068-134">Request</span></span>
<span data-ttu-id="fc068-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc068-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="fc068-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc068-136">Response</span></span>
<span data-ttu-id="fc068-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc068-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










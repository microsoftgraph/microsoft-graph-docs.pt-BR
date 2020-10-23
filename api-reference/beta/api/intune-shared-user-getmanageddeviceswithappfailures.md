---
title: função getManagedDevicesWithAppFailures
description: Recupera a lista de dispositivos com aplicativos com falha
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bfebed249e997b87d7af3b3ceeb05c82fc757e6b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702919"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="980ef-103">função getManagedDevicesWithAppFailures</span><span class="sxs-lookup"><span data-stu-id="980ef-103">getManagedDevicesWithAppFailures function</span></span>

<span data-ttu-id="980ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="980ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="980ef-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="980ef-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="980ef-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="980ef-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="980ef-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="980ef-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="980ef-108">Recupera a lista de dispositivos com aplicativos com falha</span><span class="sxs-lookup"><span data-stu-id="980ef-108">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="980ef-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="980ef-109">Prerequisites</span></span>
<span data-ttu-id="980ef-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="980ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="980ef-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="980ef-112">Permission type</span></span>|<span data-ttu-id="980ef-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="980ef-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="980ef-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="980ef-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="980ef-115">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="980ef-115">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="980ef-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="980ef-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="980ef-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="980ef-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="980ef-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="980ef-118">Not supported.</span></span>|
|<span data-ttu-id="980ef-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="980ef-119">Application</span></span>||
| <span data-ttu-id="980ef-120">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="980ef-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="980ef-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="980ef-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="980ef-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="980ef-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="980ef-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="980ef-123">Request headers</span></span>
|<span data-ttu-id="980ef-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="980ef-124">Header</span></span>|<span data-ttu-id="980ef-125">Valor</span><span class="sxs-lookup"><span data-stu-id="980ef-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="980ef-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="980ef-126">Authorization</span></span>|<span data-ttu-id="980ef-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="980ef-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="980ef-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="980ef-128">Accept</span></span>|<span data-ttu-id="980ef-129">application/json</span><span class="sxs-lookup"><span data-stu-id="980ef-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="980ef-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="980ef-130">Request body</span></span>
<span data-ttu-id="980ef-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="980ef-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="980ef-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="980ef-132">Response</span></span>
<span data-ttu-id="980ef-133">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="980ef-133">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="980ef-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="980ef-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="980ef-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="980ef-135">Request</span></span>
<span data-ttu-id="980ef-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="980ef-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="980ef-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="980ef-137">Response</span></span>
<span data-ttu-id="980ef-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="980ef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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














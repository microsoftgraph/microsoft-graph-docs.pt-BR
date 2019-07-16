---
title: função getManagedDevicesWithAppFailures
description: Recupera a lista de dispositivos com aplicativos com falha
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 576ce331a3339222877c63471ece0faee6f17982
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741238"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="c6f1a-103">função getManagedDevicesWithAppFailures</span><span class="sxs-lookup"><span data-stu-id="c6f1a-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="c6f1a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6f1a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6f1a-106">Recupera a lista de dispositivos com aplicativos com falha</span><span class="sxs-lookup"><span data-stu-id="c6f1a-106">Retrieves the list of devices with failed apps</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6f1a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c6f1a-107">Prerequisites</span></span>
<span data-ttu-id="c6f1a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6f1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6f1a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6f1a-110">Permission type</span></span>|<span data-ttu-id="c6f1a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c6f1a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6f1a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6f1a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6f1a-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6f1a-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c6f1a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6f1a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6f1a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-115">Not supported.</span></span>|
|<span data-ttu-id="c6f1a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6f1a-116">Application</span></span>|<span data-ttu-id="c6f1a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6f1a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6f1a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="c6f1a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6f1a-119">Request headers</span></span>
|<span data-ttu-id="c6f1a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6f1a-120">Header</span></span>|<span data-ttu-id="c6f1a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c6f1a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6f1a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6f1a-122">Authorization</span></span>|<span data-ttu-id="c6f1a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6f1a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c6f1a-124">Accept</span></span>|<span data-ttu-id="c6f1a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6f1a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6f1a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6f1a-126">Request body</span></span>
<span data-ttu-id="c6f1a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6f1a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6f1a-128">Response</span></span>
<span data-ttu-id="c6f1a-129">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-129">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6f1a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6f1a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6f1a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6f1a-131">Request</span></span>
<span data-ttu-id="c6f1a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="c6f1a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6f1a-133">Response</span></span>
<span data-ttu-id="c6f1a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






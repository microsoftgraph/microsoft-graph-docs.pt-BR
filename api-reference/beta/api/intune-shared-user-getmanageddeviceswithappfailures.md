---
title: função getManagedDevicesWithAppFailures
description: Recupera a lista de dispositivos com aplicativos com falha
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 44296ba60db476bd7c407ea4fbbc727ffca465ca
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172209"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="bbf0e-103">função getManagedDevicesWithAppFailures</span><span class="sxs-lookup"><span data-stu-id="bbf0e-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="bbf0e-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bbf0e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bbf0e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bbf0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bbf0e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bbf0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbf0e-107">Recupera a lista de dispositivos com aplicativos com falha</span><span class="sxs-lookup"><span data-stu-id="bbf0e-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bbf0e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bbf0e-108">Prerequisites</span></span>
<span data-ttu-id="bbf0e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbf0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="bbf0e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbf0e-111">Permission type</span></span>|<span data-ttu-id="bbf0e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bbf0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbf0e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbf0e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bbf0e-114">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="bbf0e-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="bbf0e-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbf0e-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="bbf0e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbf0e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbf0e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbf0e-117">Not supported.</span></span>|
|<span data-ttu-id="bbf0e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbf0e-118">Application</span></span>|<span data-ttu-id="bbf0e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbf0e-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbf0e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbf0e-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="bbf0e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf0e-121">Request headers</span></span>
|<span data-ttu-id="bbf0e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bbf0e-122">Header</span></span>|<span data-ttu-id="bbf0e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="bbf0e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbf0e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbf0e-124">Authorization</span></span>|<span data-ttu-id="bbf0e-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbf0e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbf0e-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bbf0e-126">Accept</span></span>|<span data-ttu-id="bbf0e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bbf0e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbf0e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf0e-128">Request body</span></span>
<span data-ttu-id="bbf0e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bbf0e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbf0e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf0e-130">Response</span></span>
<span data-ttu-id="bbf0e-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbf0e-131">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbf0e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbf0e-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="bbf0e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf0e-133">Request</span></span>
<span data-ttu-id="bbf0e-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbf0e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="bbf0e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf0e-135">Response</span></span>
<span data-ttu-id="bbf0e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbf0e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






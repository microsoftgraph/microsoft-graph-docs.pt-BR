---
title: função getManagedDevicesWithAppFailures
description: Recupera a lista de dispositivos com aplicativos com falha
author: tfitzmac
ms.openlocfilehash: 147ee26644c3e2c425f70434516e13b03407891b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352952"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="a3b6d-103">função getManagedDevicesWithAppFailures</span><span class="sxs-lookup"><span data-stu-id="a3b6d-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="a3b6d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a3b6d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3b6d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a3b6d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3b6d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a3b6d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3b6d-107">Recupera a lista de dispositivos com aplicativos com falha</span><span class="sxs-lookup"><span data-stu-id="a3b6d-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3b6d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a3b6d-108">Prerequisites</span></span>
<span data-ttu-id="a3b6d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3b6d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3b6d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3b6d-111">Permission type</span></span>|<span data-ttu-id="a3b6d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a3b6d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3b6d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3b6d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a3b6d-114">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="a3b6d-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="a3b6d-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3b6d-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a3b6d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3b6d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3b6d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3b6d-117">Not supported.</span></span>|
|<span data-ttu-id="a3b6d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3b6d-118">Application</span></span>|<span data-ttu-id="a3b6d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3b6d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3b6d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3b6d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="a3b6d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3b6d-121">Request headers</span></span>
|<span data-ttu-id="a3b6d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3b6d-122">Header</span></span>|<span data-ttu-id="a3b6d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a3b6d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3b6d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3b6d-124">Authorization</span></span>|<span data-ttu-id="a3b6d-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3b6d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3b6d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a3b6d-126">Accept</span></span>|<span data-ttu-id="a3b6d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a3b6d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3b6d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3b6d-128">Request body</span></span>
<span data-ttu-id="a3b6d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3b6d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3b6d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3b6d-130">Response</span></span>
<span data-ttu-id="a3b6d-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3b6d-131">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3b6d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3b6d-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3b6d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3b6d-133">Request</span></span>
<span data-ttu-id="a3b6d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3b6d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="a3b6d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3b6d-135">Response</span></span>
<span data-ttu-id="a3b6d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3b6d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






---
title: Lista deviceManagementScripts
description: Lista as propriedades e os relacionamentos dos objetos deviceManagementScript.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7c98ed25e43a0bb7990f900de816ee54a44c3da7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863634"
---
# <a name="list-devicemanagementscripts"></a><span data-ttu-id="f2702-103">Lista deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="f2702-103">List deviceManagementScripts</span></span>

> <span data-ttu-id="f2702-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f2702-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2702-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f2702-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2702-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f2702-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2702-107">Lista as propriedades e os relacionamentos dos objetos [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="f2702-107">List properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2702-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2702-108">Prerequisites</span></span>
<span data-ttu-id="f2702-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2702-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2702-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2702-111">Permission type</span></span>|<span data-ttu-id="f2702-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2702-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2702-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2702-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2702-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2702-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f2702-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2702-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2702-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2702-116">Not supported.</span></span>|
|<span data-ttu-id="f2702-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2702-117">Application</span></span>|<span data-ttu-id="f2702-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2702-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2702-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2702-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="f2702-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2702-120">Request headers</span></span>
|<span data-ttu-id="f2702-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2702-121">Header</span></span>|<span data-ttu-id="f2702-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2702-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2702-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2702-123">Authorization</span></span>|<span data-ttu-id="f2702-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2702-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2702-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2702-125">Accept</span></span>|<span data-ttu-id="f2702-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2702-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2702-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2702-127">Request body</span></span>
<span data-ttu-id="f2702-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2702-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2702-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2702-129">Response</span></span>
<span data-ttu-id="f2702-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2702-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2702-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2702-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f2702-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2702-132">Request</span></span>
<span data-ttu-id="f2702-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2702-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### <a name="response"></a><span data-ttu-id="f2702-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2702-134">Response</span></span>
<span data-ttu-id="f2702-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2702-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScript",
      "id": "59ea4525-4525-59ea-2545-ea592545ea59",
      "displayName": "Display Name value",
      "description": "Description value",
      "runSchedule": {
        "@odata.type": "microsoft.graph.runSchedule"
      },
      "scriptContent": "c2NyaXB0Q29udGVudA==",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "runAsAccount": "user",
      "enforceSignatureCheck": true,
      "fileName": "File Name value"
    }
  ]
}
```






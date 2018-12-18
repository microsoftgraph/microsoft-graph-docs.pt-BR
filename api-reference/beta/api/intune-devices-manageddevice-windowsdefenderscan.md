---
title: Ação windowsDefenderScan
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: d64ce1e595717d99608547ff4622d35d22d18552
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305086"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="ed8ec-103">Ação windowsDefenderScan</span><span class="sxs-lookup"><span data-stu-id="ed8ec-103">windowsDefenderScan action</span></span>

> <span data-ttu-id="ed8ec-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed8ec-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed8ec-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed8ec-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ed8ec-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed8ec-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed8ec-108">Prerequisites</span></span>
<span data-ttu-id="ed8ec-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed8ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed8ec-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed8ec-111">Permission type</span></span>|<span data-ttu-id="ed8ec-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed8ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed8ec-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed8ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed8ec-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ed8ec-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="ed8ec-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed8ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed8ec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-116">Not supported.</span></span>|
|<span data-ttu-id="ed8ec-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed8ec-117">Application</span></span>|<span data-ttu-id="ed8ec-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed8ec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed8ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="ed8ec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed8ec-120">Request headers</span></span>
|<span data-ttu-id="ed8ec-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed8ec-121">Header</span></span>|<span data-ttu-id="ed8ec-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ed8ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed8ec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed8ec-123">Authorization</span></span>|<span data-ttu-id="ed8ec-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed8ec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ed8ec-125">Accept</span></span>|<span data-ttu-id="ed8ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed8ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed8ec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed8ec-127">Request body</span></span>
<span data-ttu-id="ed8ec-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ed8ec-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ed8ec-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed8ec-130">Property</span></span>|<span data-ttu-id="ed8ec-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed8ec-131">Type</span></span>|<span data-ttu-id="ed8ec-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed8ec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed8ec-133">quickScan</span><span class="sxs-lookup"><span data-stu-id="ed8ec-133">quickScan</span></span>|<span data-ttu-id="ed8ec-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="ed8ec-134">Boolean</span></span>|<span data-ttu-id="ed8ec-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ed8ec-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ed8ec-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed8ec-136">Response</span></span>
<span data-ttu-id="ed8ec-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ed8ec-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed8ec-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed8ec-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed8ec-139">Request</span></span>
<span data-ttu-id="ed8ec-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="ed8ec-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed8ec-141">Response</span></span>
<span data-ttu-id="ed8ec-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






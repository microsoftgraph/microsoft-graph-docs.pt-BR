---
title: ação de enableLostMode
description: Habilitar o modo perdido
ms.openlocfilehash: de49cffccf3f87e91644a33128dfdfaa74b3f233
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037009"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="b3208-103">ação de enableLostMode</span><span class="sxs-lookup"><span data-stu-id="b3208-103">enableLostMode action</span></span>

> <span data-ttu-id="b3208-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b3208-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3208-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b3208-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3208-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b3208-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3208-107">Habilitar o modo perdido</span><span class="sxs-lookup"><span data-stu-id="b3208-107">Enable lost mode</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3208-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3208-108">Prerequisites</span></span>
<span data-ttu-id="b3208-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3208-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3208-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3208-111">Permission type</span></span>|<span data-ttu-id="b3208-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b3208-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3208-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3208-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3208-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="b3208-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="b3208-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3208-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3208-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3208-116">Not supported.</span></span>|
|<span data-ttu-id="b3208-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3208-117">Application</span></span>|<span data-ttu-id="b3208-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3208-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3208-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3208-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/enableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="b3208-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3208-120">Request headers</span></span>
|<span data-ttu-id="b3208-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3208-121">Header</span></span>|<span data-ttu-id="b3208-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b3208-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3208-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3208-123">Authorization</span></span>|<span data-ttu-id="b3208-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3208-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3208-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b3208-125">Accept</span></span>|<span data-ttu-id="b3208-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3208-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3208-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3208-127">Request body</span></span>
<span data-ttu-id="b3208-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b3208-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b3208-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b3208-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b3208-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3208-130">Property</span></span>|<span data-ttu-id="b3208-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3208-131">Type</span></span>|<span data-ttu-id="b3208-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3208-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3208-133">mensagem</span><span class="sxs-lookup"><span data-stu-id="b3208-133">message</span></span>|<span data-ttu-id="b3208-134">String</span><span class="sxs-lookup"><span data-stu-id="b3208-134">String</span></span>|<span data-ttu-id="b3208-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b3208-135">Not yet documented</span></span>|
|<span data-ttu-id="b3208-136">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="b3208-136">phoneNumber</span></span>|<span data-ttu-id="b3208-137">String</span><span class="sxs-lookup"><span data-stu-id="b3208-137">String</span></span>|<span data-ttu-id="b3208-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b3208-138">Not yet documented</span></span>|
|<span data-ttu-id="b3208-139">rodapé</span><span class="sxs-lookup"><span data-stu-id="b3208-139">footer</span></span>|<span data-ttu-id="b3208-140">String</span><span class="sxs-lookup"><span data-stu-id="b3208-140">String</span></span>|<span data-ttu-id="b3208-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b3208-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b3208-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3208-142">Response</span></span>
<span data-ttu-id="b3208-143">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b3208-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b3208-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3208-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3208-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3208-145">Request</span></span>
<span data-ttu-id="b3208-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3208-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/enableLostMode

Content-type: application/json
Content-length: 103

{
  "message": "Message value",
  "phoneNumber": "Phone Number value",
  "footer": "Footer value"
}
```

### <a name="response"></a><span data-ttu-id="b3208-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3208-147">Response</span></span>
<span data-ttu-id="b3208-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3208-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






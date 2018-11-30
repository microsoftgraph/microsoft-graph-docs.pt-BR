---
title: Ação wipeManagedAppRegistrationsByDeviceTag
description: Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.
ms.openlocfilehash: d6f56fa50b3162ecaebc0bb1adb02af3b4b0e9f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005976"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="e59ee-103">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="e59ee-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>



> <span data-ttu-id="e59ee-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e59ee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e59ee-105">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="e59ee-105">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e59ee-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e59ee-106">Prerequisites</span></span>
<span data-ttu-id="e59ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e59ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e59ee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e59ee-109">Permission type</span></span>|<span data-ttu-id="e59ee-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e59ee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e59ee-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e59ee-111">Delegated (work or school account)</span></span>| <span data-ttu-id="e59ee-112">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="e59ee-112">_varies by context_</span></span> |
| <span data-ttu-id="e59ee-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="e59ee-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="e59ee-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e59ee-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="e59ee-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e59ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e59ee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e59ee-116">Not supported.</span></span>|
|<span data-ttu-id="e59ee-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e59ee-117">Application</span></span>|<span data-ttu-id="e59ee-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e59ee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e59ee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e59ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="e59ee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e59ee-120">Request headers</span></span>
|<span data-ttu-id="e59ee-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e59ee-121">Header</span></span>|<span data-ttu-id="e59ee-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e59ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e59ee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e59ee-123">Authorization</span></span>|<span data-ttu-id="e59ee-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e59ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e59ee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e59ee-125">Accept</span></span>|<span data-ttu-id="e59ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e59ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e59ee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e59ee-127">Request body</span></span>
<span data-ttu-id="e59ee-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e59ee-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e59ee-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="e59ee-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e59ee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e59ee-130">Property</span></span>|<span data-ttu-id="e59ee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e59ee-131">Type</span></span>|<span data-ttu-id="e59ee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e59ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e59ee-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="e59ee-133">deviceTag</span></span>|<span data-ttu-id="e59ee-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e59ee-134">String</span></span>|<span data-ttu-id="e59ee-135">marca de dispositivo</span><span class="sxs-lookup"><span data-stu-id="e59ee-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="e59ee-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e59ee-136">Response</span></span>
<span data-ttu-id="e59ee-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e59ee-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e59ee-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e59ee-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="e59ee-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e59ee-139">Request</span></span>
<span data-ttu-id="e59ee-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e59ee-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="e59ee-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e59ee-141">Response</span></span>
<span data-ttu-id="e59ee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e59ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




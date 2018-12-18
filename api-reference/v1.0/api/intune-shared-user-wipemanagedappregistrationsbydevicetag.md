---
title: Ação wipeManagedAppRegistrationsByDeviceTag
description: Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.
author: tfitzmac
ms.openlocfilehash: 227d702d217669215894c6e6c0cfd3fa67075277
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326380"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="d9d32-103">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="d9d32-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>



> <span data-ttu-id="d9d32-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d9d32-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9d32-105">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="d9d32-105">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9d32-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9d32-106">Prerequisites</span></span>
<span data-ttu-id="d9d32-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9d32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9d32-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9d32-109">Permission type</span></span>|<span data-ttu-id="d9d32-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9d32-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9d32-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9d32-111">Delegated (work or school account)</span></span>| <span data-ttu-id="d9d32-112">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="d9d32-112">_varies by context_</span></span> |
| <span data-ttu-id="d9d32-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="d9d32-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="d9d32-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9d32-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="d9d32-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9d32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9d32-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9d32-116">Not supported.</span></span>|
|<span data-ttu-id="d9d32-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9d32-117">Application</span></span>|<span data-ttu-id="d9d32-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9d32-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9d32-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9d32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="d9d32-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d32-120">Request headers</span></span>
|<span data-ttu-id="d9d32-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9d32-121">Header</span></span>|<span data-ttu-id="d9d32-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d9d32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9d32-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9d32-123">Authorization</span></span>|<span data-ttu-id="d9d32-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9d32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9d32-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d9d32-125">Accept</span></span>|<span data-ttu-id="d9d32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9d32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9d32-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d32-127">Request body</span></span>
<span data-ttu-id="d9d32-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d9d32-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d9d32-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d9d32-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d9d32-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9d32-130">Property</span></span>|<span data-ttu-id="d9d32-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9d32-131">Type</span></span>|<span data-ttu-id="d9d32-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9d32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9d32-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="d9d32-133">deviceTag</span></span>|<span data-ttu-id="d9d32-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9d32-134">String</span></span>|<span data-ttu-id="d9d32-135">marca de dispositivo</span><span class="sxs-lookup"><span data-stu-id="d9d32-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="d9d32-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9d32-136">Response</span></span>
<span data-ttu-id="d9d32-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d9d32-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d9d32-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9d32-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9d32-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d32-139">Request</span></span>
<span data-ttu-id="d9d32-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9d32-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="d9d32-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9d32-141">Response</span></span>
<span data-ttu-id="d9d32-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9d32-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




---
title: Ação cleanWindowsDevice
description: Limpar dispositivo Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6ea625b2b91a819b64157c83b529cf336b73ab78
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753698"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="904a6-103">Ação cleanWindowsDevice</span><span class="sxs-lookup"><span data-stu-id="904a6-103">cleanWindowsDevice action</span></span>

<span data-ttu-id="904a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="904a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="904a6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="904a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="904a6-106">Limpar dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="904a6-106">Clean Windows device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="904a6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="904a6-107">Prerequisites</span></span>
<span data-ttu-id="904a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="904a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="904a6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="904a6-110">Permission type</span></span>|<span data-ttu-id="904a6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="904a6-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="904a6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="904a6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="904a6-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="904a6-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="904a6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="904a6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="904a6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="904a6-115">Not supported.</span></span>|
|<span data-ttu-id="904a6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="904a6-116">Application</span></span>|<span data-ttu-id="904a6-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="904a6-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="904a6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="904a6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="904a6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="904a6-119">Request headers</span></span>
|<span data-ttu-id="904a6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="904a6-120">Header</span></span>|<span data-ttu-id="904a6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="904a6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="904a6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="904a6-122">Authorization</span></span>|<span data-ttu-id="904a6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="904a6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="904a6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="904a6-124">Accept</span></span>|<span data-ttu-id="904a6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="904a6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="904a6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="904a6-126">Request body</span></span>
<span data-ttu-id="904a6-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="904a6-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="904a6-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="904a6-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="904a6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="904a6-129">Property</span></span>|<span data-ttu-id="904a6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="904a6-130">Type</span></span>|<span data-ttu-id="904a6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="904a6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="904a6-132">keepUserData</span><span class="sxs-lookup"><span data-stu-id="904a6-132">keepUserData</span></span>|<span data-ttu-id="904a6-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="904a6-133">Boolean</span></span>|<span data-ttu-id="904a6-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="904a6-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="904a6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="904a6-135">Response</span></span>
<span data-ttu-id="904a6-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="904a6-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="904a6-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="904a6-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="904a6-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="904a6-138">Request</span></span>
<span data-ttu-id="904a6-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="904a6-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="904a6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="904a6-140">Response</span></span>
<span data-ttu-id="904a6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="904a6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





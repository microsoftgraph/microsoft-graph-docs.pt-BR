---
title: ação assignUserToDevice
description: Atribui o usuário a dispositivos autopilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 377cd1d1323a4f9973c49d4fb1c9a8b8ebd62616
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752864"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="3a27c-103">ação assignUserToDevice</span><span class="sxs-lookup"><span data-stu-id="3a27c-103">assignUserToDevice action</span></span>

<span data-ttu-id="3a27c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a27c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a27c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a27c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a27c-106">Atribui o usuário a dispositivos autopilot.</span><span class="sxs-lookup"><span data-stu-id="3a27c-106">Assigns user to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a27c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3a27c-107">Prerequisites</span></span>
<span data-ttu-id="3a27c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a27c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a27c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a27c-110">Permission type</span></span>|<span data-ttu-id="3a27c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a27c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a27c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a27c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3a27c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a27c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3a27c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a27c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a27c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a27c-115">Not supported.</span></span>|
|<span data-ttu-id="3a27c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a27c-116">Application</span></span>|<span data-ttu-id="3a27c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a27c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a27c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a27c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="3a27c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a27c-119">Request headers</span></span>
|<span data-ttu-id="3a27c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a27c-120">Header</span></span>|<span data-ttu-id="3a27c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3a27c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a27c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a27c-122">Authorization</span></span>|<span data-ttu-id="3a27c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a27c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a27c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3a27c-124">Accept</span></span>|<span data-ttu-id="3a27c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3a27c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a27c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a27c-126">Request body</span></span>
<span data-ttu-id="3a27c-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3a27c-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3a27c-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3a27c-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3a27c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a27c-129">Property</span></span>|<span data-ttu-id="3a27c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a27c-130">Type</span></span>|<span data-ttu-id="3a27c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a27c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a27c-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3a27c-132">userPrincipalName</span></span>|<span data-ttu-id="3a27c-133">String</span><span class="sxs-lookup"><span data-stu-id="3a27c-133">String</span></span>|<span data-ttu-id="3a27c-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3a27c-134">Not yet documented</span></span>|
|<span data-ttu-id="3a27c-135">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="3a27c-135">addressableUserName</span></span>|<span data-ttu-id="3a27c-136">String</span><span class="sxs-lookup"><span data-stu-id="3a27c-136">String</span></span>|<span data-ttu-id="3a27c-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3a27c-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3a27c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a27c-138">Response</span></span>
<span data-ttu-id="3a27c-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3a27c-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3a27c-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a27c-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a27c-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a27c-141">Request</span></span>
<span data-ttu-id="3a27c-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a27c-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="3a27c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a27c-143">Response</span></span>
<span data-ttu-id="3a27c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a27c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





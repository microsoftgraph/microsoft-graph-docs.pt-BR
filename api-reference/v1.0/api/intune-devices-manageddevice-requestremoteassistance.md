---
title: Ação requestRemoteAssistance
description: Solicitar assistência remota
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01f71756c82c6a4f6b7bbf8d020407a2c03a7238
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450541"
---
# <a name="requestremoteassistance-action"></a><span data-ttu-id="7c837-103">Ação requestRemoteAssistance</span><span class="sxs-lookup"><span data-stu-id="7c837-103">requestRemoteAssistance action</span></span>

<span data-ttu-id="7c837-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c837-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c837-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c837-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c837-106">Solicitar assistência remota</span><span class="sxs-lookup"><span data-stu-id="7c837-106">Request remote assistance</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c837-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c837-107">Prerequisites</span></span>
<span data-ttu-id="7c837-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c837-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c837-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c837-110">Permission type</span></span>|<span data-ttu-id="7c837-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7c837-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c837-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c837-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c837-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c837-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7c837-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c837-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c837-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c837-115">Not supported.</span></span>|
|<span data-ttu-id="7c837-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c837-116">Application</span></span>|<span data-ttu-id="7c837-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c837-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c837-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c837-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

## <a name="request-headers"></a><span data-ttu-id="7c837-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c837-119">Request headers</span></span>
|<span data-ttu-id="7c837-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c837-120">Header</span></span>|<span data-ttu-id="7c837-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7c837-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c837-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c837-122">Authorization</span></span>|<span data-ttu-id="7c837-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c837-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c837-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c837-124">Accept</span></span>|<span data-ttu-id="7c837-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c837-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c837-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c837-126">Request body</span></span>
<span data-ttu-id="7c837-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c837-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c837-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c837-128">Response</span></span>
<span data-ttu-id="7c837-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7c837-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7c837-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c837-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c837-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c837-131">Request</span></span>
<span data-ttu-id="7c837-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c837-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

### <a name="response"></a><span data-ttu-id="7c837-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c837-133">Response</span></span>
<span data-ttu-id="7c837-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c837-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







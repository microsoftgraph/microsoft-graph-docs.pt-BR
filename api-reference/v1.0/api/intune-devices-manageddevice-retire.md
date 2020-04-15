---
title: Ação desativar
description: Desativa um dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 289f39d275bd7052169c0f9fd28d5db70f7fc03b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450487"
---
# <a name="retire-action"></a><span data-ttu-id="040dd-103">Ação retire</span><span class="sxs-lookup"><span data-stu-id="040dd-103">retire action</span></span>

<span data-ttu-id="040dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="040dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="040dd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="040dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="040dd-106">Desativa um dispositivo</span><span class="sxs-lookup"><span data-stu-id="040dd-106">Retire a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="040dd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="040dd-107">Prerequisites</span></span>
<span data-ttu-id="040dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="040dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="040dd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="040dd-110">Permission type</span></span>|<span data-ttu-id="040dd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="040dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="040dd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="040dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="040dd-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="040dd-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="040dd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="040dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="040dd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="040dd-115">Not supported.</span></span>|
|<span data-ttu-id="040dd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="040dd-116">Application</span></span>|<span data-ttu-id="040dd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="040dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="040dd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="040dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/retire
POST /deviceManagement/managedDevices/{managedDeviceId}/retire
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/retire
```

## <a name="request-headers"></a><span data-ttu-id="040dd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="040dd-119">Request headers</span></span>
|<span data-ttu-id="040dd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="040dd-120">Header</span></span>|<span data-ttu-id="040dd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="040dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="040dd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="040dd-122">Authorization</span></span>|<span data-ttu-id="040dd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="040dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="040dd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="040dd-124">Accept</span></span>|<span data-ttu-id="040dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="040dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="040dd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="040dd-126">Request body</span></span>
<span data-ttu-id="040dd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="040dd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="040dd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="040dd-128">Response</span></span>
<span data-ttu-id="040dd-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="040dd-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="040dd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="040dd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="040dd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="040dd-131">Request</span></span>
<span data-ttu-id="040dd-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="040dd-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/retire
```

### <a name="response"></a><span data-ttu-id="040dd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="040dd-133">Response</span></span>
<span data-ttu-id="040dd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="040dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







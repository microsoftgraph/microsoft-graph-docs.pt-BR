---
title: Ação windowsDefenderUpdateSignatures
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 42744627444c6e2c2e322c87ae3f604e0a15a95f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52745762"
---
# <a name="windowsdefenderupdatesignatures-action"></a><span data-ttu-id="124cc-103">Ação windowsDefenderUpdateSignatures</span><span class="sxs-lookup"><span data-stu-id="124cc-103">windowsDefenderUpdateSignatures action</span></span>

<span data-ttu-id="124cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="124cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="124cc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="124cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="124cc-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="124cc-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="124cc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="124cc-107">Prerequisites</span></span>
<span data-ttu-id="124cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="124cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="124cc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="124cc-110">Permission type</span></span>|<span data-ttu-id="124cc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="124cc-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="124cc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="124cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="124cc-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="124cc-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="124cc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="124cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="124cc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="124cc-115">Not supported.</span></span>|
|<span data-ttu-id="124cc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="124cc-116">Application</span></span>|<span data-ttu-id="124cc-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="124cc-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="124cc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="124cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

## <a name="request-headers"></a><span data-ttu-id="124cc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="124cc-119">Request headers</span></span>
|<span data-ttu-id="124cc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="124cc-120">Header</span></span>|<span data-ttu-id="124cc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="124cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="124cc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="124cc-122">Authorization</span></span>|<span data-ttu-id="124cc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="124cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="124cc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="124cc-124">Accept</span></span>|<span data-ttu-id="124cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="124cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="124cc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="124cc-126">Request body</span></span>
<span data-ttu-id="124cc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="124cc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="124cc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="124cc-128">Response</span></span>
<span data-ttu-id="124cc-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="124cc-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="124cc-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="124cc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="124cc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="124cc-131">Request</span></span>
<span data-ttu-id="124cc-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="124cc-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

### <a name="response"></a><span data-ttu-id="124cc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="124cc-133">Response</span></span>
<span data-ttu-id="124cc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="124cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





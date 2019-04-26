---
title: Ação resetPasscode
description: Redefinir senha
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 87edea2b37f61ec05ce491d1d09697b9b1c77b6b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556708"
---
# <a name="resetpasscode-action"></a><span data-ttu-id="ceb36-103">Ação resetPasscode</span><span class="sxs-lookup"><span data-stu-id="ceb36-103">resetPasscode action</span></span>

> <span data-ttu-id="ceb36-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ceb36-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ceb36-105">Redefinir senha</span><span class="sxs-lookup"><span data-stu-id="ceb36-105">Reset passcode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ceb36-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ceb36-106">Prerequisites</span></span>
<span data-ttu-id="ceb36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceb36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ceb36-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ceb36-109">Permission type</span></span>|<span data-ttu-id="ceb36-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ceb36-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ceb36-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ceb36-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ceb36-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ceb36-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="ceb36-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ceb36-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ceb36-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ceb36-114">Not supported.</span></span>|
|<span data-ttu-id="ceb36-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ceb36-115">Application</span></span>|<span data-ttu-id="ceb36-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ceb36-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ceb36-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ceb36-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/resetPasscode
POST /deviceManagement/managedDevices/{managedDeviceId}/resetPasscode
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/resetPasscode
```

## <a name="request-headers"></a><span data-ttu-id="ceb36-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ceb36-118">Request headers</span></span>
|<span data-ttu-id="ceb36-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ceb36-119">Header</span></span>|<span data-ttu-id="ceb36-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ceb36-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ceb36-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ceb36-121">Authorization</span></span>|<span data-ttu-id="ceb36-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ceb36-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ceb36-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ceb36-123">Accept</span></span>|<span data-ttu-id="ceb36-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ceb36-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ceb36-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ceb36-125">Request body</span></span>
<span data-ttu-id="ceb36-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ceb36-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ceb36-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceb36-127">Response</span></span>
<span data-ttu-id="ceb36-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ceb36-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ceb36-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ceb36-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ceb36-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ceb36-130">Request</span></span>
<span data-ttu-id="ceb36-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ceb36-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/resetPasscode
```

### <a name="response"></a><span data-ttu-id="ceb36-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceb36-132">Response</span></span>
<span data-ttu-id="ceb36-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ceb36-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




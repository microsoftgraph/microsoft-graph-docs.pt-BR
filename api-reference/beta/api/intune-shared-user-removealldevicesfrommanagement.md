---
title: Ação removeAllDevicesFromManagement
description: Desativa todos os dispositivos de gerenciamento deste usuário
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 77376044c7df41b2a6e001d0313e88498ba5121f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865072"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="163ff-103">Ação removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="163ff-103">removeAllDevicesFromManagement action</span></span>

<span data-ttu-id="163ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="163ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="163ff-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="163ff-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="163ff-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="163ff-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="163ff-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="163ff-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="163ff-108">Desativa todos os dispositivos de gerenciamento deste usuário</span><span class="sxs-lookup"><span data-stu-id="163ff-108">Retire all devices from management for this user</span></span>
## <a name="prerequisites"></a><span data-ttu-id="163ff-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="163ff-109">Prerequisites</span></span>
<span data-ttu-id="163ff-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="163ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="163ff-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="163ff-112">Permission type</span></span>|<span data-ttu-id="163ff-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="163ff-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="163ff-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="163ff-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="163ff-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="163ff-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="163ff-116">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="163ff-116">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="163ff-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="163ff-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="163ff-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="163ff-118">Not supported.</span></span>|
|<span data-ttu-id="163ff-119">Application</span><span class="sxs-lookup"><span data-stu-id="163ff-119">Application</span></span>||
| <span data-ttu-id="163ff-120">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="163ff-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="163ff-121">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="163ff-121">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="163ff-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="163ff-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="163ff-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="163ff-123">Request headers</span></span>
|<span data-ttu-id="163ff-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="163ff-124">Header</span></span>|<span data-ttu-id="163ff-125">Valor</span><span class="sxs-lookup"><span data-stu-id="163ff-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="163ff-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="163ff-126">Authorization</span></span>|<span data-ttu-id="163ff-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="163ff-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="163ff-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="163ff-128">Accept</span></span>|<span data-ttu-id="163ff-129">application/json</span><span class="sxs-lookup"><span data-stu-id="163ff-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="163ff-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="163ff-130">Request body</span></span>
<span data-ttu-id="163ff-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="163ff-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="163ff-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="163ff-132">Response</span></span>
<span data-ttu-id="163ff-133">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="163ff-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="163ff-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="163ff-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="163ff-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="163ff-135">Request</span></span>
<span data-ttu-id="163ff-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="163ff-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="163ff-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="163ff-137">Response</span></span>
<span data-ttu-id="163ff-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="163ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```













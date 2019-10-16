---
title: Ação removeAllDevicesFromManagement
description: Desativa todos os dispositivos de gerenciamento deste usuário
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9de22e32170f8907aa7fc030e49bf89324fc667b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536865"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="b8810-103">Ação removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="b8810-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="b8810-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b8810-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b8810-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b8810-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8810-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8810-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8810-107">Desativa todos os dispositivos de gerenciamento deste usuário</span><span class="sxs-lookup"><span data-stu-id="b8810-107">Retire all devices from management for this user</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8810-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8810-108">Prerequisites</span></span>
<span data-ttu-id="b8810-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8810-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8810-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8810-111">Permission type</span></span>|<span data-ttu-id="b8810-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b8810-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8810-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8810-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b8810-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="b8810-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b8810-115">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="b8810-115">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="b8810-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8810-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8810-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8810-117">Not supported.</span></span>|
|<span data-ttu-id="b8810-118">Application</span><span class="sxs-lookup"><span data-stu-id="b8810-118">Application</span></span>||
| <span data-ttu-id="b8810-119">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="b8810-119">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b8810-120">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="b8810-120">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8810-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8810-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="b8810-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8810-122">Request headers</span></span>
|<span data-ttu-id="b8810-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8810-123">Header</span></span>|<span data-ttu-id="b8810-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b8810-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8810-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8810-125">Authorization</span></span>|<span data-ttu-id="b8810-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8810-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8810-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8810-127">Accept</span></span>|<span data-ttu-id="b8810-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b8810-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8810-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8810-129">Request body</span></span>
<span data-ttu-id="b8810-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8810-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8810-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8810-131">Response</span></span>
<span data-ttu-id="b8810-132">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b8810-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b8810-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8810-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8810-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8810-134">Request</span></span>
<span data-ttu-id="b8810-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8810-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="b8810-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8810-136">Response</span></span>
<span data-ttu-id="b8810-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8810-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```












---
title: Ação removeAllDevicesFromManagement
description: Desativa todos os dispositivos de gerenciamento deste usuário
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 40baa470968c10bbe26af1d8397306f5b9e3f736
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252795"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="37c84-103">Ação removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="37c84-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="37c84-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37c84-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37c84-105">Desativa todos os dispositivos de gerenciamento deste usuário</span><span class="sxs-lookup"><span data-stu-id="37c84-105">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37c84-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37c84-106">Prerequisites</span></span>
<span data-ttu-id="37c84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37c84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37c84-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37c84-109">Permission type</span></span>|<span data-ttu-id="37c84-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37c84-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37c84-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37c84-111">Delegated (work or school account)</span></span>| <span data-ttu-id="37c84-112">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="37c84-112">_varies by context_</span></span> |
| <span data-ttu-id="37c84-113">&nbsp;&nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="37c84-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="37c84-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="37c84-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="37c84-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37c84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37c84-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37c84-116">Not supported.</span></span>|
|<span data-ttu-id="37c84-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37c84-117">Application</span></span>|<span data-ttu-id="37c84-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37c84-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37c84-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37c84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="37c84-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37c84-120">Request headers</span></span>
|<span data-ttu-id="37c84-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37c84-121">Header</span></span>|<span data-ttu-id="37c84-122">Valor</span><span class="sxs-lookup"><span data-stu-id="37c84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37c84-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="37c84-123">Authorization</span></span>|<span data-ttu-id="37c84-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37c84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37c84-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="37c84-125">Accept</span></span>|<span data-ttu-id="37c84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37c84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37c84-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37c84-127">Request body</span></span>
<span data-ttu-id="37c84-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37c84-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37c84-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="37c84-129">Response</span></span>
<span data-ttu-id="37c84-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="37c84-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="37c84-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37c84-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="37c84-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37c84-132">Request</span></span>
<span data-ttu-id="37c84-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37c84-133">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="37c84-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="37c84-134">Response</span></span>
<span data-ttu-id="37c84-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37c84-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




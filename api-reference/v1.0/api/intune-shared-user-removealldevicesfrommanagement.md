---
title: Ação removeAllDevicesFromManagement
description: Desativa todos os dispositivos de gerenciamento deste usuário
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d35b852ef9694a2e9d8f427ba3bbb98cb2b4c26a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025761"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="707ad-103">Ação removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="707ad-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="707ad-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="707ad-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="707ad-105">Desativa todos os dispositivos de gerenciamento deste usuário</span><span class="sxs-lookup"><span data-stu-id="707ad-105">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="707ad-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="707ad-106">Prerequisites</span></span>
<span data-ttu-id="707ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="707ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="707ad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="707ad-109">Permission type</span></span>|<span data-ttu-id="707ad-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="707ad-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="707ad-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="707ad-111">Delegated (work or school account)</span></span>| <span data-ttu-id="707ad-112">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="707ad-112">_varies by context_</span></span> |
| <span data-ttu-id="707ad-113">&nbsp;&nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="707ad-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="707ad-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="707ad-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="707ad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="707ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="707ad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="707ad-116">Not supported.</span></span>|
|<span data-ttu-id="707ad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="707ad-117">Application</span></span>|<span data-ttu-id="707ad-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="707ad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="707ad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="707ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="707ad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="707ad-120">Request headers</span></span>
|<span data-ttu-id="707ad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="707ad-121">Header</span></span>|<span data-ttu-id="707ad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="707ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="707ad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="707ad-123">Authorization</span></span>|<span data-ttu-id="707ad-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="707ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="707ad-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="707ad-125">Accept</span></span>|<span data-ttu-id="707ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="707ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="707ad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="707ad-127">Request body</span></span>
<span data-ttu-id="707ad-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="707ad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="707ad-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="707ad-129">Response</span></span>
<span data-ttu-id="707ad-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="707ad-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="707ad-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="707ad-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="707ad-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="707ad-132">Request</span></span>
<span data-ttu-id="707ad-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="707ad-133">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="707ad-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="707ad-134">Response</span></span>
<span data-ttu-id="707ad-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="707ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




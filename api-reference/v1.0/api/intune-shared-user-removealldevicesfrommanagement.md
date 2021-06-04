---
title: Ação removeAllDevicesFromManagement
description: Desativa todos os dispositivos de gerenciamento deste usuário
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2072d8022aa95c82dcdc6deae727c4fd7f64b7fd
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732321"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="d2052-103">Ação removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="d2052-103">removeAllDevicesFromManagement action</span></span>

<span data-ttu-id="d2052-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2052-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2052-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2052-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2052-106">Desativa todos os dispositivos de gerenciamento deste usuário</span><span class="sxs-lookup"><span data-stu-id="d2052-106">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2052-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d2052-107">Prerequisites</span></span>
<span data-ttu-id="d2052-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2052-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2052-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2052-110">Permission type</span></span>|<span data-ttu-id="d2052-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d2052-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2052-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2052-112">Delegated (work or school account)</span></span>| <span data-ttu-id="d2052-113">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="d2052-113">_varies by context_</span></span> |
| <span data-ttu-id="d2052-114">&nbsp;&nbsp;Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="d2052-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="d2052-115">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="d2052-115">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="d2052-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2052-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2052-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2052-117">Not supported.</span></span>|
|<span data-ttu-id="d2052-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2052-118">Application</span></span>|<span data-ttu-id="d2052-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2052-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2052-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2052-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="d2052-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2052-121">Request headers</span></span>
|<span data-ttu-id="d2052-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d2052-122">Header</span></span>|<span data-ttu-id="d2052-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d2052-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2052-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2052-124">Authorization</span></span>|<span data-ttu-id="d2052-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2052-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2052-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d2052-126">Accept</span></span>|<span data-ttu-id="d2052-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d2052-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2052-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2052-128">Request body</span></span>
<span data-ttu-id="d2052-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2052-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2052-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2052-130">Response</span></span>
<span data-ttu-id="d2052-131">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d2052-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d2052-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2052-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2052-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2052-133">Request</span></span>
<span data-ttu-id="d2052-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2052-134">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="d2052-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2052-135">Response</span></span>
<span data-ttu-id="d2052-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2052-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```










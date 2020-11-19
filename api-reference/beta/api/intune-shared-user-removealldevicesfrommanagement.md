---
title: Ação removeAllDevicesFromManagement
description: Desativa todos os dispositivos de gerenciamento deste usuário
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8d62358ce3f95ce21f5553ff6984c404f578d7d7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49303850"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="e4779-103">Ação removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="e4779-103">removeAllDevicesFromManagement action</span></span>

<span data-ttu-id="e4779-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4779-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4779-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e4779-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e4779-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e4779-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4779-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4779-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4779-108">Desativa todos os dispositivos de gerenciamento deste usuário</span><span class="sxs-lookup"><span data-stu-id="e4779-108">Retire all devices from management for this user</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4779-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4779-109">Prerequisites</span></span>
<span data-ttu-id="e4779-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4779-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4779-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4779-112">Permission type</span></span>|<span data-ttu-id="e4779-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4779-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4779-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4779-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e4779-115">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="e4779-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e4779-116">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e4779-116">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="e4779-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4779-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4779-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4779-118">Not supported.</span></span>|
|<span data-ttu-id="e4779-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4779-119">Application</span></span>||
| <span data-ttu-id="e4779-120">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="e4779-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e4779-121">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e4779-121">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4779-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4779-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="e4779-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4779-123">Request headers</span></span>
|<span data-ttu-id="e4779-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4779-124">Header</span></span>|<span data-ttu-id="e4779-125">Valor</span><span class="sxs-lookup"><span data-stu-id="e4779-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4779-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4779-126">Authorization</span></span>|<span data-ttu-id="e4779-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4779-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4779-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e4779-128">Accept</span></span>|<span data-ttu-id="e4779-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e4779-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4779-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4779-130">Request body</span></span>
<span data-ttu-id="e4779-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4779-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4779-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4779-132">Response</span></span>
<span data-ttu-id="e4779-133">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e4779-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e4779-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4779-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4779-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4779-135">Request</span></span>
<span data-ttu-id="e4779-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4779-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="e4779-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4779-137">Response</span></span>
<span data-ttu-id="e4779-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4779-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```













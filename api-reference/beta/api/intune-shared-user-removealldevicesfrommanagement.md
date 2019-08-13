---
title: Ação removeAllDevicesFromManagement
description: Desativa todos os dispositivos de gerenciamento deste usuário
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1916fcd5bd30ad67b12c93a81108eb62a532fde9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350598"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="ca16b-103">Ação removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="ca16b-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="ca16b-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ca16b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ca16b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ca16b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca16b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca16b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca16b-107">Desativa todos os dispositivos de gerenciamento deste usuário</span><span class="sxs-lookup"><span data-stu-id="ca16b-107">Retire all devices from management for this user</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca16b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca16b-108">Prerequisites</span></span>
<span data-ttu-id="ca16b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca16b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca16b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca16b-111">Permission type</span></span>|<span data-ttu-id="ca16b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ca16b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca16b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca16b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ca16b-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="ca16b-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ca16b-115">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ca16b-115">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="ca16b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca16b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca16b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca16b-117">Not supported.</span></span>|
|<span data-ttu-id="ca16b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca16b-118">Application</span></span>|<span data-ttu-id="ca16b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca16b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca16b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca16b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="ca16b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca16b-121">Request headers</span></span>
|<span data-ttu-id="ca16b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca16b-122">Header</span></span>|<span data-ttu-id="ca16b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ca16b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca16b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca16b-124">Authorization</span></span>|<span data-ttu-id="ca16b-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca16b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca16b-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca16b-126">Accept</span></span>|<span data-ttu-id="ca16b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ca16b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca16b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca16b-128">Request body</span></span>
<span data-ttu-id="ca16b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca16b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca16b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca16b-130">Response</span></span>
<span data-ttu-id="ca16b-131">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ca16b-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ca16b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca16b-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca16b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca16b-133">Request</span></span>
<span data-ttu-id="ca16b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca16b-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="ca16b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca16b-135">Response</span></span>
<span data-ttu-id="ca16b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca16b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









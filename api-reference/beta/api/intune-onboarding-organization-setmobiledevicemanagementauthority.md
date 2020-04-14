---
title: Ação setMobileDeviceManagementAuthority
description: Define uma autoridade de gerenciamento de dispositivo móvel
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5c716cc4adad6c8e8a07f762f39c468b396280dd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461768"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="e31b8-103">ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="e31b8-103">setMobileDeviceManagementAuthority action</span></span>

<span data-ttu-id="e31b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e31b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e31b8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e31b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e31b8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e31b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e31b8-107">Define uma autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="e31b8-107">Set mobile device management authority</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e31b8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e31b8-108">Prerequisites</span></span>
<span data-ttu-id="e31b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e31b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e31b8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e31b8-111">Permission type</span></span>|<span data-ttu-id="e31b8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e31b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e31b8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e31b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e31b8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e31b8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e31b8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e31b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e31b8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e31b8-116">Not supported.</span></span>|
|<span data-ttu-id="e31b8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e31b8-117">Application</span></span>|<span data-ttu-id="e31b8-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e31b8-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e31b8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e31b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="e31b8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e31b8-120">Request headers</span></span>
|<span data-ttu-id="e31b8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e31b8-121">Header</span></span>|<span data-ttu-id="e31b8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e31b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e31b8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e31b8-123">Authorization</span></span>|<span data-ttu-id="e31b8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e31b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e31b8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e31b8-125">Accept</span></span>|<span data-ttu-id="e31b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e31b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e31b8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e31b8-127">Request body</span></span>
<span data-ttu-id="e31b8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e31b8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e31b8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e31b8-129">Response</span></span>
<span data-ttu-id="e31b8-130">Se tiver êxito, esta ação retorna o código de resposta `200 OK` e a Int32 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e31b8-130">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e31b8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e31b8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e31b8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e31b8-132">Request</span></span>
<span data-ttu-id="e31b8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e31b8-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="e31b8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e31b8-134">Response</span></span>
<span data-ttu-id="e31b8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e31b8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```




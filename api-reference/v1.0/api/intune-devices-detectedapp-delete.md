---
title: Excluir detectedApp
description: Exclui detectedApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7192d562d6a3390a5d45623ddd4529794fe6b3be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018726"
---
# <a name="delete-detectedapp"></a><span data-ttu-id="24b94-103">Excluir detectedApp</span><span class="sxs-lookup"><span data-stu-id="24b94-103">Delete detectedApp</span></span>

> <span data-ttu-id="24b94-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="24b94-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24b94-105">Exclui [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="24b94-105">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24b94-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="24b94-106">Prerequisites</span></span>
<span data-ttu-id="24b94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24b94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24b94-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24b94-109">Permission type</span></span>|<span data-ttu-id="24b94-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="24b94-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24b94-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24b94-111">Delegated (work or school account)</span></span>|<span data-ttu-id="24b94-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24b94-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="24b94-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24b94-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24b94-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24b94-114">Not supported.</span></span>|
|<span data-ttu-id="24b94-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24b94-115">Application</span></span>|<span data-ttu-id="24b94-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24b94-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24b94-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24b94-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="24b94-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24b94-118">Request headers</span></span>
|<span data-ttu-id="24b94-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24b94-119">Header</span></span>|<span data-ttu-id="24b94-120">Valor</span><span class="sxs-lookup"><span data-stu-id="24b94-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24b94-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="24b94-121">Authorization</span></span>|<span data-ttu-id="24b94-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24b94-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24b94-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="24b94-123">Accept</span></span>|<span data-ttu-id="24b94-124">application/json</span><span class="sxs-lookup"><span data-stu-id="24b94-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24b94-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24b94-125">Request body</span></span>
<span data-ttu-id="24b94-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24b94-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24b94-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="24b94-127">Response</span></span>
<span data-ttu-id="24b94-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="24b94-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="24b94-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24b94-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="24b94-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24b94-130">Request</span></span>
<span data-ttu-id="24b94-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24b94-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}
```

### <a name="response"></a><span data-ttu-id="24b94-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="24b94-132">Response</span></span>
<span data-ttu-id="24b94-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24b94-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




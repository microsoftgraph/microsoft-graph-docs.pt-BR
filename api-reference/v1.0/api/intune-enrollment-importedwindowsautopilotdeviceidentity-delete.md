---
title: Excluir importedWindowsAutopilotDeviceIdentity
description: Exclui uma importedWindowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8dfcadb755f3eae632fc9a84dde283c955c082fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020822"
---
# <a name="delete-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="0c92c-103">Excluir importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="0c92c-103">Delete importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="0c92c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c92c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c92c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c92c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c92c-106">Exclui uma [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="0c92c-106">Deletes a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c92c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c92c-107">Prerequisites</span></span>
<span data-ttu-id="0c92c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c92c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c92c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c92c-110">Permission type</span></span>|<span data-ttu-id="0c92c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c92c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c92c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c92c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c92c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c92c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0c92c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c92c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c92c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c92c-115">Not supported.</span></span>|
|<span data-ttu-id="0c92c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c92c-116">Application</span></span>|<span data-ttu-id="0c92c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c92c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c92c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c92c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
DELETE /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="0c92c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c92c-119">Request headers</span></span>
|<span data-ttu-id="0c92c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c92c-120">Header</span></span>|<span data-ttu-id="0c92c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0c92c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c92c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c92c-122">Authorization</span></span>|<span data-ttu-id="0c92c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c92c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c92c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c92c-124">Accept</span></span>|<span data-ttu-id="0c92c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c92c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c92c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c92c-126">Request body</span></span>
<span data-ttu-id="0c92c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0c92c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c92c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c92c-128">Response</span></span>
<span data-ttu-id="0c92c-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0c92c-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0c92c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c92c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c92c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c92c-131">Request</span></span>
<span data-ttu-id="0c92c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c92c-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="0c92c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c92c-133">Response</span></span>
<span data-ttu-id="0c92c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c92c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```










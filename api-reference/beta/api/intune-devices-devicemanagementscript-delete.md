---
title: Excluir deviceManagementScript
description: Exclui deviceManagementScript.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0ad8ba7f998d0ecf86b318c5c65b82c02ebe77c5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958267"
---
# <a name="delete-devicemanagementscript"></a><span data-ttu-id="43683-103">Excluir deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="43683-103">Delete deviceManagementScript</span></span>

> <span data-ttu-id="43683-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="43683-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43683-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43683-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43683-106">Exclui [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="43683-106">Deletes a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43683-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43683-107">Prerequisites</span></span>
<span data-ttu-id="43683-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43683-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43683-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43683-110">Permission type</span></span>|<span data-ttu-id="43683-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="43683-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43683-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43683-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43683-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43683-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="43683-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43683-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43683-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43683-115">Not supported.</span></span>|
|<span data-ttu-id="43683-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43683-116">Application</span></span>|<span data-ttu-id="43683-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43683-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43683-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43683-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="43683-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43683-119">Request headers</span></span>
|<span data-ttu-id="43683-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43683-120">Header</span></span>|<span data-ttu-id="43683-121">Valor</span><span class="sxs-lookup"><span data-stu-id="43683-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43683-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="43683-122">Authorization</span></span>|<span data-ttu-id="43683-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43683-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43683-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43683-124">Accept</span></span>|<span data-ttu-id="43683-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43683-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43683-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43683-126">Request body</span></span>
<span data-ttu-id="43683-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43683-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43683-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="43683-128">Response</span></span>
<span data-ttu-id="43683-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="43683-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="43683-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43683-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="43683-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43683-131">Request</span></span>
<span data-ttu-id="43683-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43683-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a><span data-ttu-id="43683-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="43683-133">Response</span></span>
<span data-ttu-id="43683-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43683-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





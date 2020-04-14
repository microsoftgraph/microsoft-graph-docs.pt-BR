---
title: Excluir deviceShellScript
description: Exclui deviceShellScript.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 712494917f90e7a5a3ffa0250152fa8e7d24054d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43425588"
---
# <a name="delete-deviceshellscript"></a><span data-ttu-id="a1126-103">Excluir deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="a1126-103">Delete deviceShellScript</span></span>

<span data-ttu-id="a1126-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1126-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1126-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1126-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1126-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1126-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1126-107">Exclui [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span><span class="sxs-lookup"><span data-stu-id="a1126-107">Deletes a [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1126-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1126-108">Prerequisites</span></span>
<span data-ttu-id="a1126-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1126-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1126-111">Permission type</span></span>|<span data-ttu-id="a1126-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1126-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1126-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1126-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1126-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1126-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a1126-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1126-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1126-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1126-116">Not supported.</span></span>|
|<span data-ttu-id="a1126-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1126-117">Application</span></span>|<span data-ttu-id="a1126-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1126-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1126-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1126-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceShellScripts/{deviceShellScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="a1126-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1126-120">Request headers</span></span>
|<span data-ttu-id="a1126-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1126-121">Header</span></span>|<span data-ttu-id="a1126-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a1126-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1126-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1126-123">Authorization</span></span>|<span data-ttu-id="a1126-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1126-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1126-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1126-125">Accept</span></span>|<span data-ttu-id="a1126-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1126-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1126-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1126-127">Request body</span></span>
<span data-ttu-id="a1126-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1126-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1126-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1126-129">Response</span></span>
<span data-ttu-id="a1126-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a1126-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a1126-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1126-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1126-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1126-132">Request</span></span>
<span data-ttu-id="a1126-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1126-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}
```

### <a name="response"></a><span data-ttu-id="a1126-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1126-134">Response</span></span>
<span data-ttu-id="a1126-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1126-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




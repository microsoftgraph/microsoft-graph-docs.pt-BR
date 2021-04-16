---
title: Excluir deviceManagementScript
description: Exclui um deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 664c30b6889e2d2cb90ddb60ae8118c8cf92e8bb
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867802"
---
# <a name="delete-devicemanagementscript"></a><span data-ttu-id="f25bb-103">Excluir deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="f25bb-103">Delete deviceManagementScript</span></span>

<span data-ttu-id="f25bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f25bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f25bb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f25bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f25bb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f25bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f25bb-107">Exclui um [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="f25bb-107">Deletes a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f25bb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f25bb-108">Prerequisites</span></span>
<span data-ttu-id="f25bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f25bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f25bb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f25bb-111">Permission type</span></span>|<span data-ttu-id="f25bb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f25bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f25bb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f25bb-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f25bb-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f25bb-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="f25bb-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f25bb-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="f25bb-116">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="f25bb-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f25bb-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f25bb-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f25bb-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f25bb-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f25bb-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f25bb-119">Not supported.</span></span>|
|<span data-ttu-id="f25bb-120">Application</span><span class="sxs-lookup"><span data-stu-id="f25bb-120">Application</span></span>||
| <span data-ttu-id="f25bb-121">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f25bb-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="f25bb-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f25bb-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="f25bb-123">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="f25bb-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f25bb-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f25bb-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f25bb-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f25bb-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="f25bb-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f25bb-126">Request headers</span></span>
|<span data-ttu-id="f25bb-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f25bb-127">Header</span></span>|<span data-ttu-id="f25bb-128">Valor</span><span class="sxs-lookup"><span data-stu-id="f25bb-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f25bb-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="f25bb-129">Authorization</span></span>|<span data-ttu-id="f25bb-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f25bb-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f25bb-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f25bb-131">Accept</span></span>|<span data-ttu-id="f25bb-132">application/json</span><span class="sxs-lookup"><span data-stu-id="f25bb-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f25bb-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f25bb-133">Request body</span></span>
<span data-ttu-id="f25bb-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f25bb-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f25bb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f25bb-135">Response</span></span>
<span data-ttu-id="f25bb-136">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f25bb-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f25bb-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f25bb-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f25bb-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f25bb-138">Request</span></span>
<span data-ttu-id="f25bb-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f25bb-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a><span data-ttu-id="f25bb-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f25bb-140">Response</span></span>
<span data-ttu-id="f25bb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f25bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








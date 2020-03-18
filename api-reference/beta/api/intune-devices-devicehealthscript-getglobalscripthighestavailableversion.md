---
title: ação getGlobalScriptHighestAvailableVersion
description: Atualizar o script de integridade do dispositivo proprietário
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c8067183162b4e445f040b94736bb664122792c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814614"
---
# <a name="getglobalscripthighestavailableversion-action"></a><span data-ttu-id="1a3f9-103">ação getGlobalScriptHighestAvailableVersion</span><span class="sxs-lookup"><span data-stu-id="1a3f9-103">getGlobalScriptHighestAvailableVersion action</span></span>

> <span data-ttu-id="1a3f9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1a3f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a3f9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a3f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a3f9-106">Atualizar o script de integridade do dispositivo proprietário</span><span class="sxs-lookup"><span data-stu-id="1a3f9-106">Update the Proprietary Device Health Script</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a3f9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1a3f9-107">Prerequisites</span></span>
<span data-ttu-id="1a3f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a3f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a3f9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a3f9-110">Permission type</span></span>|<span data-ttu-id="1a3f9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1a3f9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a3f9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a3f9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a3f9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a3f9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1a3f9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a3f9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a3f9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a3f9-115">Not supported.</span></span>|
|<span data-ttu-id="1a3f9-116">Application</span><span class="sxs-lookup"><span data-stu-id="1a3f9-116">Application</span></span>|<span data-ttu-id="1a3f9-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a3f9-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a3f9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a3f9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getGlobalScriptHighestAvailableVersion
```

## <a name="request-headers"></a><span data-ttu-id="1a3f9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a3f9-119">Request headers</span></span>
|<span data-ttu-id="1a3f9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1a3f9-120">Header</span></span>|<span data-ttu-id="1a3f9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1a3f9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a3f9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a3f9-122">Authorization</span></span>|<span data-ttu-id="1a3f9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a3f9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a3f9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1a3f9-124">Accept</span></span>|<span data-ttu-id="1a3f9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a3f9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a3f9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a3f9-126">Request body</span></span>
<span data-ttu-id="1a3f9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1a3f9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a3f9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a3f9-128">Response</span></span>
<span data-ttu-id="1a3f9-129">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a3f9-129">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a3f9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a3f9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a3f9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a3f9-131">Request</span></span>
<span data-ttu-id="1a3f9-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a3f9-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getGlobalScriptHighestAvailableVersion
```

### <a name="response"></a><span data-ttu-id="1a3f9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a3f9-133">Response</span></span>
<span data-ttu-id="1a3f9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a3f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 68

{
  "value": "Get Global Script Highest Available Version value"
}
```





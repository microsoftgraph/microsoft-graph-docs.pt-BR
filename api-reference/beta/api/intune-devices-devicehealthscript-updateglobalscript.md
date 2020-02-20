---
title: ação updateGlobalScript
description: Atualizar o script de integridade do dispositivo proprietário
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 366fdcb5f19d6e50dfa5936c45c984cddbfb6d6d
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162180"
---
# <a name="updateglobalscript-action"></a><span data-ttu-id="e4426-103">ação updateGlobalScript</span><span class="sxs-lookup"><span data-stu-id="e4426-103">updateGlobalScript action</span></span>

> <span data-ttu-id="e4426-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4426-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4426-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4426-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4426-106">Atualizar o script de integridade do dispositivo proprietário</span><span class="sxs-lookup"><span data-stu-id="e4426-106">Update the Proprietary Device Health Script</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4426-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4426-107">Prerequisites</span></span>
<span data-ttu-id="e4426-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4426-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4426-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4426-110">Permission type</span></span>|<span data-ttu-id="e4426-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4426-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4426-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4426-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4426-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4426-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e4426-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4426-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4426-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4426-115">Not supported.</span></span>|
|<span data-ttu-id="e4426-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4426-116">Application</span></span>|<span data-ttu-id="e4426-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4426-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4426-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4426-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/updateGlobalScript
```

## <a name="request-headers"></a><span data-ttu-id="e4426-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4426-119">Request headers</span></span>
|<span data-ttu-id="e4426-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4426-120">Header</span></span>|<span data-ttu-id="e4426-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e4426-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4426-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4426-122">Authorization</span></span>|<span data-ttu-id="e4426-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4426-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4426-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e4426-124">Accept</span></span>|<span data-ttu-id="e4426-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4426-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4426-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4426-126">Request body</span></span>
<span data-ttu-id="e4426-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e4426-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e4426-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="e4426-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e4426-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4426-129">Property</span></span>|<span data-ttu-id="e4426-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4426-130">Type</span></span>|<span data-ttu-id="e4426-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4426-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4426-132">versão</span><span class="sxs-lookup"><span data-stu-id="e4426-132">version</span></span>|<span data-ttu-id="e4426-133">String</span><span class="sxs-lookup"><span data-stu-id="e4426-133">String</span></span>|<span data-ttu-id="e4426-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e4426-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e4426-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4426-135">Response</span></span>
<span data-ttu-id="e4426-136">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4426-136">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4426-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4426-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4426-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4426-138">Request</span></span>
<span data-ttu-id="e4426-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4426-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/updateGlobalScript

Content-type: application/json
Content-length: 34

{
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="e4426-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4426-140">Response</span></span>
<span data-ttu-id="e4426-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4426-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 45

{
  "value": "Update Global Script value"
}
```






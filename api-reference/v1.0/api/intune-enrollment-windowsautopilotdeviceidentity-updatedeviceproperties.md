---
title: Ação updateDeviceProperties
description: Atualiza as propriedades em dispositivos do Autopilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ecdca46463b608b3aa2cacd55c4f4cbe00afe0c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752855"
---
# <a name="updatedeviceproperties-action"></a><span data-ttu-id="61796-103">Ação updateDeviceProperties</span><span class="sxs-lookup"><span data-stu-id="61796-103">updateDeviceProperties action</span></span>

<span data-ttu-id="61796-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61796-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61796-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61796-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61796-106">Atualiza as propriedades em dispositivos do Autopilot.</span><span class="sxs-lookup"><span data-stu-id="61796-106">Updates properties on Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61796-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61796-107">Prerequisites</span></span>
<span data-ttu-id="61796-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61796-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61796-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61796-110">Permission type</span></span>|<span data-ttu-id="61796-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61796-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61796-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61796-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61796-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61796-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="61796-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61796-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61796-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61796-115">Not supported.</span></span>|
|<span data-ttu-id="61796-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61796-116">Application</span></span>|<span data-ttu-id="61796-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61796-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61796-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61796-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties
```

## <a name="request-headers"></a><span data-ttu-id="61796-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61796-119">Request headers</span></span>
|<span data-ttu-id="61796-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61796-120">Header</span></span>|<span data-ttu-id="61796-121">Valor</span><span class="sxs-lookup"><span data-stu-id="61796-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61796-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="61796-122">Authorization</span></span>|<span data-ttu-id="61796-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61796-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61796-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61796-124">Accept</span></span>|<span data-ttu-id="61796-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61796-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61796-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61796-126">Request body</span></span>
<span data-ttu-id="61796-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="61796-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="61796-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="61796-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="61796-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61796-129">Property</span></span>|<span data-ttu-id="61796-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="61796-130">Type</span></span>|<span data-ttu-id="61796-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="61796-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61796-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="61796-132">userPrincipalName</span></span>|<span data-ttu-id="61796-133">String</span><span class="sxs-lookup"><span data-stu-id="61796-133">String</span></span>|<span data-ttu-id="61796-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="61796-134">Not yet documented</span></span>|
|<span data-ttu-id="61796-135">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="61796-135">addressableUserName</span></span>|<span data-ttu-id="61796-136">String</span><span class="sxs-lookup"><span data-stu-id="61796-136">String</span></span>|<span data-ttu-id="61796-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="61796-137">Not yet documented</span></span>|
|<span data-ttu-id="61796-138">groupTag</span><span class="sxs-lookup"><span data-stu-id="61796-138">groupTag</span></span>|<span data-ttu-id="61796-139">String</span><span class="sxs-lookup"><span data-stu-id="61796-139">String</span></span>|<span data-ttu-id="61796-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="61796-140">Not yet documented</span></span>|
|<span data-ttu-id="61796-141">displayName</span><span class="sxs-lookup"><span data-stu-id="61796-141">displayName</span></span>|<span data-ttu-id="61796-142">String</span><span class="sxs-lookup"><span data-stu-id="61796-142">String</span></span>|<span data-ttu-id="61796-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="61796-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="61796-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="61796-144">Response</span></span>
<span data-ttu-id="61796-145">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="61796-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="61796-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61796-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="61796-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61796-147">Request</span></span>
<span data-ttu-id="61796-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61796-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties

Content-type: application/json
Content-length: 187

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value",
  "groupTag": "Group Tag value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="61796-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="61796-149">Response</span></span>
<span data-ttu-id="61796-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61796-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





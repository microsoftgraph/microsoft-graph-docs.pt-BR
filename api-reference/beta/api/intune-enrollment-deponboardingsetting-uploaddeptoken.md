---
title: Ação uploadDepToken
description: Carrega um novo token do programa de registro de dispositivos
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ecba652effa9a5ac5cdfd2f220025342578f1646
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050539"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="efb6a-103">Ação uploadDepToken</span><span class="sxs-lookup"><span data-stu-id="efb6a-103">uploadDepToken action</span></span>

<span data-ttu-id="efb6a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efb6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efb6a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="efb6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efb6a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="efb6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efb6a-107">Carrega um novo token do programa de registro de dispositivos</span><span class="sxs-lookup"><span data-stu-id="efb6a-107">Uploads a new Device Enrollment Program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efb6a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="efb6a-108">Prerequisites</span></span>
<span data-ttu-id="efb6a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efb6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efb6a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efb6a-111">Permission type</span></span>|<span data-ttu-id="efb6a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="efb6a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efb6a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efb6a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efb6a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efb6a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="efb6a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efb6a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efb6a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efb6a-116">Not supported.</span></span>|
|<span data-ttu-id="efb6a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efb6a-117">Application</span></span>|<span data-ttu-id="efb6a-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efb6a-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efb6a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efb6a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="efb6a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efb6a-120">Request headers</span></span>
|<span data-ttu-id="efb6a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="efb6a-121">Header</span></span>|<span data-ttu-id="efb6a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="efb6a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efb6a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="efb6a-123">Authorization</span></span>|<span data-ttu-id="efb6a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efb6a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efb6a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="efb6a-125">Accept</span></span>|<span data-ttu-id="efb6a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efb6a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efb6a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efb6a-127">Request body</span></span>
<span data-ttu-id="efb6a-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="efb6a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="efb6a-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="efb6a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="efb6a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efb6a-130">Property</span></span>|<span data-ttu-id="efb6a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="efb6a-131">Type</span></span>|<span data-ttu-id="efb6a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="efb6a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efb6a-133">appleId</span><span class="sxs-lookup"><span data-stu-id="efb6a-133">appleId</span></span>|<span data-ttu-id="efb6a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efb6a-134">String</span></span>|<span data-ttu-id="efb6a-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="efb6a-135">Not yet documented</span></span>|
|<span data-ttu-id="efb6a-136">depToken</span><span class="sxs-lookup"><span data-stu-id="efb6a-136">depToken</span></span>|<span data-ttu-id="efb6a-137">String</span><span class="sxs-lookup"><span data-stu-id="efb6a-137">String</span></span>|<span data-ttu-id="efb6a-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="efb6a-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="efb6a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="efb6a-139">Response</span></span>
<span data-ttu-id="efb6a-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="efb6a-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="efb6a-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efb6a-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="efb6a-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efb6a-142">Request</span></span>
<span data-ttu-id="efb6a-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efb6a-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="efb6a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="efb6a-144">Response</span></span>
<span data-ttu-id="efb6a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efb6a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







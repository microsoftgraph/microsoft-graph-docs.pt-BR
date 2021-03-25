---
title: Ação uploadDepToken
description: Carrega um novo token do Programa de Registro de Dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d302676b16f29e7f004081b78d77c4fc2a610e48
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153913"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="54128-103">Ação uploadDepToken</span><span class="sxs-lookup"><span data-stu-id="54128-103">uploadDepToken action</span></span>

<span data-ttu-id="54128-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54128-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54128-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54128-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54128-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54128-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54128-107">Carrega um novo token do Programa de Registro de Dispositivo</span><span class="sxs-lookup"><span data-stu-id="54128-107">Uploads a new Device Enrollment Program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54128-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54128-108">Prerequisites</span></span>
<span data-ttu-id="54128-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54128-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54128-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54128-111">Permission type</span></span>|<span data-ttu-id="54128-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54128-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54128-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54128-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54128-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54128-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="54128-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54128-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54128-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54128-116">Not supported.</span></span>|
|<span data-ttu-id="54128-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54128-117">Application</span></span>|<span data-ttu-id="54128-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54128-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54128-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54128-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="54128-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54128-120">Request headers</span></span>
|<span data-ttu-id="54128-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54128-121">Header</span></span>|<span data-ttu-id="54128-122">Valor</span><span class="sxs-lookup"><span data-stu-id="54128-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54128-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="54128-123">Authorization</span></span>|<span data-ttu-id="54128-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54128-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54128-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54128-125">Accept</span></span>|<span data-ttu-id="54128-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54128-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54128-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54128-127">Request body</span></span>
<span data-ttu-id="54128-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="54128-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="54128-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="54128-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="54128-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54128-130">Property</span></span>|<span data-ttu-id="54128-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="54128-131">Type</span></span>|<span data-ttu-id="54128-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="54128-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54128-133">appleId</span><span class="sxs-lookup"><span data-stu-id="54128-133">appleId</span></span>|<span data-ttu-id="54128-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54128-134">String</span></span>|<span data-ttu-id="54128-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="54128-135">Not yet documented</span></span>|
|<span data-ttu-id="54128-136">depToken</span><span class="sxs-lookup"><span data-stu-id="54128-136">depToken</span></span>|<span data-ttu-id="54128-137">String</span><span class="sxs-lookup"><span data-stu-id="54128-137">String</span></span>|<span data-ttu-id="54128-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="54128-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="54128-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="54128-139">Response</span></span>
<span data-ttu-id="54128-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="54128-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="54128-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54128-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="54128-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54128-142">Request</span></span>
<span data-ttu-id="54128-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54128-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="54128-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="54128-144">Response</span></span>
<span data-ttu-id="54128-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54128-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





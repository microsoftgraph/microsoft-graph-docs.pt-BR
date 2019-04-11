---
title: Ação uploadDepToken
description: Carrega um novo token do programa de registro de dispositivos
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 553f0156304d69af79ca957a9d05a0115a41d93a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807879"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="b2c31-103">Ação uploadDepToken</span><span class="sxs-lookup"><span data-stu-id="b2c31-103">uploadDepToken action</span></span>

> <span data-ttu-id="b2c31-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2c31-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2c31-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2c31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2c31-106">Carrega um novo token do programa de registro de dispositivos</span><span class="sxs-lookup"><span data-stu-id="b2c31-106">Uploads a new Device Enrollment Program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2c31-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2c31-107">Prerequisites</span></span>
<span data-ttu-id="b2c31-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2c31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2c31-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2c31-110">Permission type</span></span>|<span data-ttu-id="b2c31-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2c31-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2c31-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2c31-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2c31-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2c31-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b2c31-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2c31-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2c31-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2c31-115">Not supported.</span></span>|
|<span data-ttu-id="b2c31-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2c31-116">Application</span></span>|<span data-ttu-id="b2c31-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2c31-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2c31-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2c31-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="b2c31-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2c31-119">Request headers</span></span>
|<span data-ttu-id="b2c31-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2c31-120">Header</span></span>|<span data-ttu-id="b2c31-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b2c31-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2c31-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2c31-122">Authorization</span></span>|<span data-ttu-id="b2c31-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2c31-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2c31-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2c31-124">Accept</span></span>|<span data-ttu-id="b2c31-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2c31-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2c31-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2c31-126">Request body</span></span>
<span data-ttu-id="b2c31-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b2c31-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b2c31-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b2c31-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b2c31-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2c31-129">Property</span></span>|<span data-ttu-id="b2c31-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2c31-130">Type</span></span>|<span data-ttu-id="b2c31-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2c31-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2c31-132">appleId</span><span class="sxs-lookup"><span data-stu-id="b2c31-132">appleId</span></span>|<span data-ttu-id="b2c31-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2c31-133">String</span></span>|<span data-ttu-id="b2c31-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b2c31-134">Not yet documented</span></span>|
|<span data-ttu-id="b2c31-135">depToken</span><span class="sxs-lookup"><span data-stu-id="b2c31-135">depToken</span></span>|<span data-ttu-id="b2c31-136">String</span><span class="sxs-lookup"><span data-stu-id="b2c31-136">String</span></span>|<span data-ttu-id="b2c31-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b2c31-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b2c31-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2c31-138">Response</span></span>
<span data-ttu-id="b2c31-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b2c31-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b2c31-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2c31-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2c31-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2c31-141">Request</span></span>
<span data-ttu-id="b2c31-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2c31-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="b2c31-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2c31-143">Response</span></span>
<span data-ttu-id="b2c31-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2c31-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






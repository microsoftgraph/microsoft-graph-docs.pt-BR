---
title: Ação completeSignup
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f8e06f27a23de281916bbe2db330cd47323a8de3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962348"
---
# <a name="completesignup-action"></a><span data-ttu-id="7786e-103">Ação completeSignup</span><span class="sxs-lookup"><span data-stu-id="7786e-103">completeSignup action</span></span>

> <span data-ttu-id="7786e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7786e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7786e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7786e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7786e-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7786e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7786e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7786e-107">Prerequisites</span></span>
<span data-ttu-id="7786e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7786e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7786e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7786e-110">Permission type</span></span>|<span data-ttu-id="7786e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7786e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7786e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7786e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7786e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7786e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7786e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7786e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7786e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7786e-115">Not supported.</span></span>|
|<span data-ttu-id="7786e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7786e-116">Application</span></span>|<span data-ttu-id="7786e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7786e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7786e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7786e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/completeSignup
```

## <a name="request-headers"></a><span data-ttu-id="7786e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7786e-119">Request headers</span></span>
|<span data-ttu-id="7786e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7786e-120">Header</span></span>|<span data-ttu-id="7786e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7786e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7786e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7786e-122">Authorization</span></span>|<span data-ttu-id="7786e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7786e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7786e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7786e-124">Accept</span></span>|<span data-ttu-id="7786e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7786e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7786e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7786e-126">Request body</span></span>
<span data-ttu-id="7786e-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7786e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7786e-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="7786e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7786e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7786e-129">Property</span></span>|<span data-ttu-id="7786e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7786e-130">Type</span></span>|<span data-ttu-id="7786e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7786e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7786e-132">enterpriseToken</span><span class="sxs-lookup"><span data-stu-id="7786e-132">enterpriseToken</span></span>|<span data-ttu-id="7786e-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7786e-133">String</span></span>|<span data-ttu-id="7786e-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7786e-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7786e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7786e-135">Response</span></span>
<span data-ttu-id="7786e-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7786e-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7786e-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7786e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="7786e-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7786e-138">Request</span></span>
<span data-ttu-id="7786e-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7786e-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/completeSignup

Content-type: application/json
Content-length: 51

{
  "enterpriseToken": "Enterprise Token value"
}
```

### <a name="response"></a><span data-ttu-id="7786e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7786e-140">Response</span></span>
<span data-ttu-id="7786e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7786e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





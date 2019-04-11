---
title: Ação createToken
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c95d6e112c4d34ee7b593c4f34dcab08c560b25d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774082"
---
# <a name="createtoken-action"></a><span data-ttu-id="3c598-103">Ação createToken</span><span class="sxs-lookup"><span data-stu-id="3c598-103">createToken action</span></span>

> <span data-ttu-id="3c598-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c598-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c598-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c598-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c598-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3c598-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c598-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c598-107">Prerequisites</span></span>
<span data-ttu-id="3c598-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c598-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c598-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c598-110">Permission type</span></span>|<span data-ttu-id="3c598-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c598-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c598-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c598-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c598-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c598-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c598-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c598-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c598-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c598-115">Not supported.</span></span>|
|<span data-ttu-id="3c598-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c598-116">Application</span></span>|<span data-ttu-id="3c598-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c598-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c598-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c598-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}/createToken
```

## <a name="request-headers"></a><span data-ttu-id="3c598-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c598-119">Request headers</span></span>
|<span data-ttu-id="3c598-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c598-120">Header</span></span>|<span data-ttu-id="3c598-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3c598-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c598-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c598-122">Authorization</span></span>|<span data-ttu-id="3c598-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c598-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c598-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c598-124">Accept</span></span>|<span data-ttu-id="3c598-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c598-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c598-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c598-126">Request body</span></span>
<span data-ttu-id="3c598-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3c598-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3c598-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3c598-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3c598-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c598-129">Property</span></span>|<span data-ttu-id="3c598-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c598-130">Type</span></span>|<span data-ttu-id="3c598-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c598-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c598-132">tokenValidityInSeconds</span><span class="sxs-lookup"><span data-stu-id="3c598-132">tokenValidityInSeconds</span></span>|<span data-ttu-id="3c598-133">Int32</span><span class="sxs-lookup"><span data-stu-id="3c598-133">Int32</span></span>|<span data-ttu-id="3c598-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3c598-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3c598-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c598-135">Response</span></span>
<span data-ttu-id="3c598-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3c598-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3c598-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c598-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c598-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c598-138">Request</span></span>
<span data-ttu-id="3c598-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c598-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}/createToken

Content-type: application/json
Content-length: 35

{
  "tokenValidityInSeconds": 6
}
```

### <a name="response"></a><span data-ttu-id="3c598-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c598-140">Response</span></span>
<span data-ttu-id="3c598-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c598-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






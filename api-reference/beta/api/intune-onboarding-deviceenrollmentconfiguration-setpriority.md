---
title: Ação setPriority
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e5b5d9ecf2061f64018b2cd9501981e79201b514
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791569"
---
# <a name="setpriority-action"></a><span data-ttu-id="befcc-103">ação setPriority</span><span class="sxs-lookup"><span data-stu-id="befcc-103">setPriority action</span></span>

> <span data-ttu-id="befcc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="befcc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="befcc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="befcc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="befcc-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="befcc-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="befcc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="befcc-107">Prerequisites</span></span>
<span data-ttu-id="befcc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="befcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="befcc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="befcc-110">Permission type</span></span>|<span data-ttu-id="befcc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="befcc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="befcc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="befcc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="befcc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="befcc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="befcc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="befcc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="befcc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="befcc-115">Not supported.</span></span>|
|<span data-ttu-id="befcc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="befcc-116">Application</span></span>|<span data-ttu-id="befcc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="befcc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="befcc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="befcc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="befcc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="befcc-119">Request headers</span></span>
|<span data-ttu-id="befcc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="befcc-120">Header</span></span>|<span data-ttu-id="befcc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="befcc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="befcc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="befcc-122">Authorization</span></span>|<span data-ttu-id="befcc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="befcc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="befcc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="befcc-124">Accept</span></span>|<span data-ttu-id="befcc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="befcc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="befcc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="befcc-126">Request body</span></span>
<span data-ttu-id="befcc-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="befcc-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="befcc-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="befcc-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="befcc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="befcc-129">Property</span></span>|<span data-ttu-id="befcc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="befcc-130">Type</span></span>|<span data-ttu-id="befcc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="befcc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="befcc-132">Prioridade</span><span class="sxs-lookup"><span data-stu-id="befcc-132">priority</span></span>|<span data-ttu-id="befcc-133">Int32</span><span class="sxs-lookup"><span data-stu-id="befcc-133">Int32</span></span>|<span data-ttu-id="befcc-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="befcc-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="befcc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="befcc-135">Response</span></span>
<span data-ttu-id="befcc-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="befcc-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="befcc-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="befcc-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="befcc-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="befcc-138">Request</span></span>
<span data-ttu-id="befcc-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="befcc-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="befcc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="befcc-140">Response</span></span>
<span data-ttu-id="befcc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="befcc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






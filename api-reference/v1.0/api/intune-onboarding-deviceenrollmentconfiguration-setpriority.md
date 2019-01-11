---
title: Ação setPriority
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9fb5080cedb1025aa49e6195e646a7a877655f1e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826849"
---
# <a name="setpriority-action"></a><span data-ttu-id="f0dcf-103">Ação setPriority</span><span class="sxs-lookup"><span data-stu-id="f0dcf-103">setPriority action</span></span>

> <span data-ttu-id="f0dcf-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f0dcf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0dcf-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f0dcf-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0dcf-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f0dcf-106">Prerequisites</span></span>
<span data-ttu-id="f0dcf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0dcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0dcf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0dcf-109">Permission type</span></span>|<span data-ttu-id="f0dcf-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f0dcf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0dcf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0dcf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f0dcf-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0dcf-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f0dcf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0dcf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0dcf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0dcf-114">Not supported.</span></span>|
|<span data-ttu-id="f0dcf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0dcf-115">Application</span></span>|<span data-ttu-id="f0dcf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0dcf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0dcf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0dcf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="f0dcf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0dcf-118">Request headers</span></span>
|<span data-ttu-id="f0dcf-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0dcf-119">Header</span></span>|<span data-ttu-id="f0dcf-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f0dcf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0dcf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0dcf-121">Authorization</span></span>|<span data-ttu-id="f0dcf-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0dcf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0dcf-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f0dcf-123">Accept</span></span>|<span data-ttu-id="f0dcf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f0dcf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0dcf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0dcf-125">Request body</span></span>
<span data-ttu-id="f0dcf-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f0dcf-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f0dcf-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f0dcf-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f0dcf-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0dcf-128">Property</span></span>|<span data-ttu-id="f0dcf-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0dcf-129">Type</span></span>|<span data-ttu-id="f0dcf-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0dcf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0dcf-131">Prioridade</span><span class="sxs-lookup"><span data-stu-id="f0dcf-131">priority</span></span>|<span data-ttu-id="f0dcf-132">Int32</span><span class="sxs-lookup"><span data-stu-id="f0dcf-132">Int32</span></span>|<span data-ttu-id="f0dcf-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f0dcf-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f0dcf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0dcf-134">Response</span></span>
<span data-ttu-id="f0dcf-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f0dcf-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f0dcf-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0dcf-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0dcf-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0dcf-137">Request</span></span>
<span data-ttu-id="f0dcf-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0dcf-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="f0dcf-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0dcf-139">Response</span></span>
<span data-ttu-id="f0dcf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0dcf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




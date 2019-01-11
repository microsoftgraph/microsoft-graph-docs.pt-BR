---
title: função exportDeviceAndAppManagementData
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c7c4bc294d382cf1e1917a2c5a607a7c90107856
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872839"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="97617-103">função exportDeviceAndAppManagementData</span><span class="sxs-lookup"><span data-stu-id="97617-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="97617-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="97617-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97617-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="97617-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97617-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="97617-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97617-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="97617-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97617-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97617-108">Prerequisites</span></span>

<span data-ttu-id="97617-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97617-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97617-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97617-111">Permission type</span></span>|<span data-ttu-id="97617-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97617-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97617-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97617-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="97617-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="97617-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="97617-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97617-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="97617-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97617-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97617-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97617-117">Not supported.</span></span>|
|<span data-ttu-id="97617-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97617-118">Application</span></span>|<span data-ttu-id="97617-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97617-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97617-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97617-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="97617-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97617-121">Request headers</span></span>

|<span data-ttu-id="97617-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97617-122">Header</span></span>|<span data-ttu-id="97617-123">Valor</span><span class="sxs-lookup"><span data-stu-id="97617-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97617-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="97617-124">Authorization</span></span>|<span data-ttu-id="97617-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97617-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97617-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97617-126">Accept</span></span>|<span data-ttu-id="97617-127">application/json</span><span class="sxs-lookup"><span data-stu-id="97617-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97617-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97617-128">Request body</span></span>

<span data-ttu-id="97617-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="97617-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="97617-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97617-130">Property</span></span>|<span data-ttu-id="97617-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="97617-131">Type</span></span>|<span data-ttu-id="97617-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="97617-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97617-133">skip</span><span class="sxs-lookup"><span data-stu-id="97617-133">skip</span></span>|<span data-ttu-id="97617-134">Int32</span><span class="sxs-lookup"><span data-stu-id="97617-134">Int32</span></span>|<span data-ttu-id="97617-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="97617-135">Not yet documented</span></span>|
|<span data-ttu-id="97617-136">top</span><span class="sxs-lookup"><span data-stu-id="97617-136">top</span></span>|<span data-ttu-id="97617-137">Int32</span><span class="sxs-lookup"><span data-stu-id="97617-137">Int32</span></span>|<span data-ttu-id="97617-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="97617-138">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="97617-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="97617-139">Response</span></span>

<span data-ttu-id="97617-140">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97617-140">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97617-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97617-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="97617-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97617-142">Request</span></span>

<span data-ttu-id="97617-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97617-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="97617-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="97617-144">Response</span></span>

<span data-ttu-id="97617-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97617-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 143

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementData",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```




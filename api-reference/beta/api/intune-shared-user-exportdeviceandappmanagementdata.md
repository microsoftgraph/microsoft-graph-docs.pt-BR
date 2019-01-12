---
title: função exportDeviceAndAppManagementData
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5ab337ccca261dde98d609434fa7948bc07bcfca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965107"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="33aae-103">função exportDeviceAndAppManagementData</span><span class="sxs-lookup"><span data-stu-id="33aae-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="33aae-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="33aae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33aae-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="33aae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33aae-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="33aae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33aae-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="33aae-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33aae-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33aae-108">Prerequisites</span></span>

<span data-ttu-id="33aae-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33aae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33aae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33aae-111">Permission type</span></span>|<span data-ttu-id="33aae-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="33aae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33aae-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33aae-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="33aae-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="33aae-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="33aae-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33aae-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="33aae-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33aae-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33aae-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33aae-117">Not supported.</span></span>|
|<span data-ttu-id="33aae-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33aae-118">Application</span></span>|<span data-ttu-id="33aae-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33aae-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33aae-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33aae-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="33aae-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33aae-121">Request headers</span></span>

|<span data-ttu-id="33aae-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33aae-122">Header</span></span>|<span data-ttu-id="33aae-123">Valor</span><span class="sxs-lookup"><span data-stu-id="33aae-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33aae-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="33aae-124">Authorization</span></span>|<span data-ttu-id="33aae-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33aae-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33aae-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="33aae-126">Accept</span></span>|<span data-ttu-id="33aae-127">application/json</span><span class="sxs-lookup"><span data-stu-id="33aae-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33aae-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33aae-128">Request body</span></span>

<span data-ttu-id="33aae-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="33aae-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="33aae-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33aae-130">Property</span></span>|<span data-ttu-id="33aae-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="33aae-131">Type</span></span>|<span data-ttu-id="33aae-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="33aae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33aae-133">skip</span><span class="sxs-lookup"><span data-stu-id="33aae-133">skip</span></span>|<span data-ttu-id="33aae-134">Int32</span><span class="sxs-lookup"><span data-stu-id="33aae-134">Int32</span></span>|<span data-ttu-id="33aae-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="33aae-135">Not yet documented</span></span>|
|<span data-ttu-id="33aae-136">top</span><span class="sxs-lookup"><span data-stu-id="33aae-136">top</span></span>|<span data-ttu-id="33aae-137">Int32</span><span class="sxs-lookup"><span data-stu-id="33aae-137">Int32</span></span>|<span data-ttu-id="33aae-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="33aae-138">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="33aae-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="33aae-139">Response</span></span>

<span data-ttu-id="33aae-140">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33aae-140">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33aae-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33aae-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="33aae-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33aae-142">Request</span></span>

<span data-ttu-id="33aae-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33aae-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="33aae-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="33aae-144">Response</span></span>

<span data-ttu-id="33aae-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33aae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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




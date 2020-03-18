---
title: função exportDeviceAndAppManagementData
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 93c80b33a6598cd79d1f203a291cf61ff9f9d949
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800582"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="537e5-103">função exportDeviceAndAppManagementData</span><span class="sxs-lookup"><span data-stu-id="537e5-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="537e5-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="537e5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="537e5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="537e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="537e5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="537e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="537e5-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="537e5-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="537e5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="537e5-108">Prerequisites</span></span>

<span data-ttu-id="537e5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="537e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="537e5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="537e5-111">Permission type</span></span>|<span data-ttu-id="537e5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="537e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="537e5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="537e5-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="537e5-114">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="537e5-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="537e5-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="537e5-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="537e5-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="537e5-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="537e5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="537e5-117">Not supported.</span></span>|
|<span data-ttu-id="537e5-118">Application</span><span class="sxs-lookup"><span data-stu-id="537e5-118">Application</span></span>||
| <span data-ttu-id="537e5-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="537e5-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="537e5-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="537e5-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="537e5-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="537e5-121">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="537e5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="537e5-122">Request headers</span></span>

|<span data-ttu-id="537e5-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="537e5-123">Header</span></span>|<span data-ttu-id="537e5-124">Valor</span><span class="sxs-lookup"><span data-stu-id="537e5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="537e5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="537e5-125">Authorization</span></span>|<span data-ttu-id="537e5-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="537e5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="537e5-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="537e5-127">Accept</span></span>|<span data-ttu-id="537e5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="537e5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="537e5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="537e5-129">Request body</span></span>

<span data-ttu-id="537e5-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="537e5-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="537e5-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="537e5-131">Property</span></span>|<span data-ttu-id="537e5-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="537e5-132">Type</span></span>|<span data-ttu-id="537e5-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="537e5-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="537e5-134">skip</span><span class="sxs-lookup"><span data-stu-id="537e5-134">skip</span></span>|<span data-ttu-id="537e5-135">Int32</span><span class="sxs-lookup"><span data-stu-id="537e5-135">Int32</span></span>|<span data-ttu-id="537e5-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="537e5-136">Not yet documented</span></span>|
|<span data-ttu-id="537e5-137">top</span><span class="sxs-lookup"><span data-stu-id="537e5-137">top</span></span>|<span data-ttu-id="537e5-138">Int32</span><span class="sxs-lookup"><span data-stu-id="537e5-138">Int32</span></span>|<span data-ttu-id="537e5-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="537e5-139">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="537e5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="537e5-140">Response</span></span>

<span data-ttu-id="537e5-141">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="537e5-141">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="537e5-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="537e5-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="537e5-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="537e5-143">Request</span></span>

<span data-ttu-id="537e5-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="537e5-144">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="537e5-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="537e5-145">Response</span></span>

<span data-ttu-id="537e5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="537e5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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











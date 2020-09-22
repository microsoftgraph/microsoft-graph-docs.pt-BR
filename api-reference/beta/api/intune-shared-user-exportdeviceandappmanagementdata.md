---
title: função exportDeviceAndAppManagementData
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d53c84e7e127739222086848d61eb032d38d0b15
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999731"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="968a0-103">função exportDeviceAndAppManagementData</span><span class="sxs-lookup"><span data-stu-id="968a0-103">exportDeviceAndAppManagementData function</span></span>

<span data-ttu-id="968a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="968a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="968a0-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="968a0-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="968a0-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="968a0-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="968a0-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="968a0-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="968a0-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="968a0-108">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="968a0-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="968a0-109">Prerequisites</span></span>

<span data-ttu-id="968a0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="968a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="968a0-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="968a0-112">Permission type</span></span>|<span data-ttu-id="968a0-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="968a0-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="968a0-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="968a0-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="968a0-115">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="968a0-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="968a0-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="968a0-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="968a0-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="968a0-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="968a0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="968a0-118">Not supported.</span></span>|
|<span data-ttu-id="968a0-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="968a0-119">Application</span></span>||
| <span data-ttu-id="968a0-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="968a0-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="968a0-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="968a0-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="968a0-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="968a0-122">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="968a0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="968a0-123">Request headers</span></span>

|<span data-ttu-id="968a0-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="968a0-124">Header</span></span>|<span data-ttu-id="968a0-125">Valor</span><span class="sxs-lookup"><span data-stu-id="968a0-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="968a0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="968a0-126">Authorization</span></span>|<span data-ttu-id="968a0-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="968a0-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="968a0-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="968a0-128">Accept</span></span>|<span data-ttu-id="968a0-129">application/json</span><span class="sxs-lookup"><span data-stu-id="968a0-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="968a0-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="968a0-130">Request body</span></span>

<span data-ttu-id="968a0-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="968a0-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="968a0-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="968a0-132">Property</span></span>|<span data-ttu-id="968a0-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="968a0-133">Type</span></span>|<span data-ttu-id="968a0-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="968a0-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="968a0-135">skip</span><span class="sxs-lookup"><span data-stu-id="968a0-135">skip</span></span>|<span data-ttu-id="968a0-136">Int32</span><span class="sxs-lookup"><span data-stu-id="968a0-136">Int32</span></span>|<span data-ttu-id="968a0-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="968a0-137">Not yet documented</span></span>|
|<span data-ttu-id="968a0-138">top</span><span class="sxs-lookup"><span data-stu-id="968a0-138">top</span></span>|<span data-ttu-id="968a0-139">Int32</span><span class="sxs-lookup"><span data-stu-id="968a0-139">Int32</span></span>|<span data-ttu-id="968a0-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="968a0-140">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="968a0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="968a0-141">Response</span></span>

<span data-ttu-id="968a0-142">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="968a0-142">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="968a0-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="968a0-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="968a0-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="968a0-144">Request</span></span>

<span data-ttu-id="968a0-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="968a0-145">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="968a0-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="968a0-146">Response</span></span>

<span data-ttu-id="968a0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="968a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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













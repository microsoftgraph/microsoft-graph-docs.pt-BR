---
title: ação createInstance
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 66203d2de8c6c3a1a7be7172ca8e70cccd708263
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774635"
---
# <a name="createinstance-action"></a><span data-ttu-id="74bf5-103">ação createInstance</span><span class="sxs-lookup"><span data-stu-id="74bf5-103">createInstance action</span></span>

> <span data-ttu-id="74bf5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="74bf5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74bf5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="74bf5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74bf5-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="74bf5-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74bf5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="74bf5-107">Prerequisites</span></span>
<span data-ttu-id="74bf5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74bf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74bf5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74bf5-110">Permission type</span></span>|<span data-ttu-id="74bf5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="74bf5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74bf5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74bf5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74bf5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74bf5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74bf5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74bf5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74bf5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74bf5-115">Not supported.</span></span>|
|<span data-ttu-id="74bf5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74bf5-116">Application</span></span>|<span data-ttu-id="74bf5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74bf5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74bf5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74bf5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/createInstance
```

## <a name="request-headers"></a><span data-ttu-id="74bf5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74bf5-119">Request headers</span></span>
|<span data-ttu-id="74bf5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74bf5-120">Header</span></span>|<span data-ttu-id="74bf5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="74bf5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74bf5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="74bf5-122">Authorization</span></span>|<span data-ttu-id="74bf5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74bf5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74bf5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="74bf5-124">Accept</span></span>|<span data-ttu-id="74bf5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74bf5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74bf5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74bf5-126">Request body</span></span>
<span data-ttu-id="74bf5-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="74bf5-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="74bf5-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="74bf5-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="74bf5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74bf5-129">Property</span></span>|<span data-ttu-id="74bf5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="74bf5-130">Type</span></span>|<span data-ttu-id="74bf5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="74bf5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74bf5-132">displayName</span><span class="sxs-lookup"><span data-stu-id="74bf5-132">displayName</span></span>|<span data-ttu-id="74bf5-133">String</span><span class="sxs-lookup"><span data-stu-id="74bf5-133">String</span></span>|<span data-ttu-id="74bf5-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="74bf5-134">Not yet documented</span></span>|
|<span data-ttu-id="74bf5-135">description</span><span class="sxs-lookup"><span data-stu-id="74bf5-135">description</span></span>|<span data-ttu-id="74bf5-136">String</span><span class="sxs-lookup"><span data-stu-id="74bf5-136">String</span></span>|<span data-ttu-id="74bf5-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="74bf5-137">Not yet documented</span></span>|
|<span data-ttu-id="74bf5-138">settingsDelta</span><span class="sxs-lookup"><span data-stu-id="74bf5-138">settingsDelta</span></span>|<span data-ttu-id="74bf5-139">coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="74bf5-139">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="74bf5-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="74bf5-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="74bf5-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="74bf5-141">Response</span></span>
<span data-ttu-id="74bf5-142">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e um [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74bf5-142">If successful, this action returns a `200 OK` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74bf5-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74bf5-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="74bf5-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74bf5-144">Request</span></span>
<span data-ttu-id="74bf5-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74bf5-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/createInstance

Content-type: application/json
Content-length: 336

{
  "displayName": "Display Name value",
  "description": "Description value",
  "settingsDelta": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
      "id": "d68168e1-68e1-d681-e168-81d6e16881d6",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="74bf5-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="74bf5-146">Response</span></span>
<span data-ttu-id="74bf5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74bf5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 350

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntent",
    "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
    "displayName": "Display Name value",
    "description": "Description value",
    "isAssigned": true,
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "templateId": "Template Id value"
  }
}
```






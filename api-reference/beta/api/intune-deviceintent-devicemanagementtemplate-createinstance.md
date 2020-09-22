---
title: ação createInstance
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c165339bd2cdf3f6cf990b7279844737c8d4c8aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011344"
---
# <a name="createinstance-action"></a><span data-ttu-id="716bf-103">ação createInstance</span><span class="sxs-lookup"><span data-stu-id="716bf-103">createInstance action</span></span>

<span data-ttu-id="716bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="716bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="716bf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="716bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="716bf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="716bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="716bf-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="716bf-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="716bf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="716bf-108">Prerequisites</span></span>
<span data-ttu-id="716bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="716bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="716bf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="716bf-111">Permission type</span></span>|<span data-ttu-id="716bf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="716bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="716bf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="716bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="716bf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="716bf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="716bf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="716bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="716bf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="716bf-116">Not supported.</span></span>|
|<span data-ttu-id="716bf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="716bf-117">Application</span></span>|<span data-ttu-id="716bf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="716bf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="716bf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="716bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/createInstance
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}/createInstance
```

## <a name="request-headers"></a><span data-ttu-id="716bf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="716bf-120">Request headers</span></span>
|<span data-ttu-id="716bf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="716bf-121">Header</span></span>|<span data-ttu-id="716bf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="716bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="716bf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="716bf-123">Authorization</span></span>|<span data-ttu-id="716bf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="716bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="716bf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="716bf-125">Accept</span></span>|<span data-ttu-id="716bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="716bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="716bf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="716bf-127">Request body</span></span>
<span data-ttu-id="716bf-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="716bf-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="716bf-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="716bf-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="716bf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="716bf-130">Property</span></span>|<span data-ttu-id="716bf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="716bf-131">Type</span></span>|<span data-ttu-id="716bf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="716bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="716bf-133">displayName</span><span class="sxs-lookup"><span data-stu-id="716bf-133">displayName</span></span>|<span data-ttu-id="716bf-134">String</span><span class="sxs-lookup"><span data-stu-id="716bf-134">String</span></span>|<span data-ttu-id="716bf-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="716bf-135">Not yet documented</span></span>|
|<span data-ttu-id="716bf-136">description</span><span class="sxs-lookup"><span data-stu-id="716bf-136">description</span></span>|<span data-ttu-id="716bf-137">String</span><span class="sxs-lookup"><span data-stu-id="716bf-137">String</span></span>|<span data-ttu-id="716bf-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="716bf-138">Not yet documented</span></span>|
|<span data-ttu-id="716bf-139">settingsDelta</span><span class="sxs-lookup"><span data-stu-id="716bf-139">settingsDelta</span></span>|<span data-ttu-id="716bf-140">coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="716bf-140">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="716bf-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="716bf-141">Not yet documented</span></span>|
|<span data-ttu-id="716bf-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="716bf-142">roleScopeTagIds</span></span>|<span data-ttu-id="716bf-143">String collection</span><span class="sxs-lookup"><span data-stu-id="716bf-143">String collection</span></span>|<span data-ttu-id="716bf-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="716bf-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="716bf-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="716bf-145">Response</span></span>
<span data-ttu-id="716bf-146">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e um [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="716bf-146">If successful, this action returns a `200 OK` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="716bf-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="716bf-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="716bf-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="716bf-148">Request</span></span>
<span data-ttu-id="716bf-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="716bf-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/createInstance

Content-type: application/json
Content-length: 398

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
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="716bf-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="716bf-150">Response</span></span>
<span data-ttu-id="716bf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="716bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 418

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntent",
    "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
    "displayName": "Display Name value",
    "description": "Description value",
    "isAssigned": true,
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "templateId": "Template Id value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```







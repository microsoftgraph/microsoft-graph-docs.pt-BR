---
title: ação createInstance
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1ad5347cdff40f804cf9a601d02f352a9cfbda41
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49286266"
---
# <a name="createinstance-action"></a><span data-ttu-id="6ee95-103">ação createInstance</span><span class="sxs-lookup"><span data-stu-id="6ee95-103">createInstance action</span></span>

<span data-ttu-id="6ee95-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ee95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ee95-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ee95-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ee95-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ee95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ee95-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6ee95-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ee95-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6ee95-108">Prerequisites</span></span>
<span data-ttu-id="6ee95-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ee95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ee95-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ee95-111">Permission type</span></span>|<span data-ttu-id="6ee95-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6ee95-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ee95-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ee95-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ee95-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ee95-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ee95-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ee95-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ee95-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ee95-116">Not supported.</span></span>|
|<span data-ttu-id="6ee95-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ee95-117">Application</span></span>|<span data-ttu-id="6ee95-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ee95-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ee95-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ee95-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/createInstance
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}/createInstance
```

## <a name="request-headers"></a><span data-ttu-id="6ee95-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ee95-120">Request headers</span></span>
|<span data-ttu-id="6ee95-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ee95-121">Header</span></span>|<span data-ttu-id="6ee95-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6ee95-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ee95-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ee95-123">Authorization</span></span>|<span data-ttu-id="6ee95-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ee95-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ee95-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6ee95-125">Accept</span></span>|<span data-ttu-id="6ee95-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ee95-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ee95-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ee95-127">Request body</span></span>
<span data-ttu-id="6ee95-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="6ee95-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6ee95-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="6ee95-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6ee95-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ee95-130">Property</span></span>|<span data-ttu-id="6ee95-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ee95-131">Type</span></span>|<span data-ttu-id="6ee95-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ee95-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ee95-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6ee95-133">displayName</span></span>|<span data-ttu-id="6ee95-134">String</span><span class="sxs-lookup"><span data-stu-id="6ee95-134">String</span></span>|<span data-ttu-id="6ee95-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6ee95-135">Not yet documented</span></span>|
|<span data-ttu-id="6ee95-136">description</span><span class="sxs-lookup"><span data-stu-id="6ee95-136">description</span></span>|<span data-ttu-id="6ee95-137">String</span><span class="sxs-lookup"><span data-stu-id="6ee95-137">String</span></span>|<span data-ttu-id="6ee95-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6ee95-138">Not yet documented</span></span>|
|<span data-ttu-id="6ee95-139">settingsDelta</span><span class="sxs-lookup"><span data-stu-id="6ee95-139">settingsDelta</span></span>|<span data-ttu-id="6ee95-140">coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="6ee95-140">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="6ee95-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6ee95-141">Not yet documented</span></span>|
|<span data-ttu-id="6ee95-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6ee95-142">roleScopeTagIds</span></span>|<span data-ttu-id="6ee95-143">String collection</span><span class="sxs-lookup"><span data-stu-id="6ee95-143">String collection</span></span>|<span data-ttu-id="6ee95-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6ee95-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6ee95-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ee95-145">Response</span></span>
<span data-ttu-id="6ee95-146">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e um [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ee95-146">If successful, this action returns a `200 OK` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ee95-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ee95-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ee95-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ee95-148">Request</span></span>
<span data-ttu-id="6ee95-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ee95-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6ee95-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ee95-150">Response</span></span>
<span data-ttu-id="6ee95-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ee95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





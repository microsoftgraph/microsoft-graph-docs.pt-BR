---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9c76128d4b637a95a5b2bb8911608b6fd9afa857
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939862"
---
# <a name="assign-action"></a><span data-ttu-id="48f78-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="48f78-103">assign action</span></span>

> <span data-ttu-id="48f78-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48f78-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48f78-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48f78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48f78-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48f78-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48f78-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="48f78-107">Prerequisites</span></span>
<span data-ttu-id="48f78-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48f78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48f78-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48f78-110">Permission type</span></span>|<span data-ttu-id="48f78-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="48f78-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48f78-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48f78-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="48f78-113">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="48f78-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="48f78-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f78-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="48f78-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48f78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48f78-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48f78-116">Not supported.</span></span>|
|<span data-ttu-id="48f78-117">Application</span><span class="sxs-lookup"><span data-stu-id="48f78-117">Application</span></span>||
| <span data-ttu-id="48f78-118">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="48f78-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="48f78-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f78-119">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48f78-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48f78-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="48f78-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48f78-121">Request headers</span></span>
|<span data-ttu-id="48f78-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48f78-122">Header</span></span>|<span data-ttu-id="48f78-123">Valor</span><span class="sxs-lookup"><span data-stu-id="48f78-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48f78-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="48f78-124">Authorization</span></span>|<span data-ttu-id="48f78-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48f78-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48f78-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="48f78-126">Accept</span></span>|<span data-ttu-id="48f78-127">application/json</span><span class="sxs-lookup"><span data-stu-id="48f78-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48f78-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48f78-128">Request body</span></span>
<span data-ttu-id="48f78-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="48f78-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="48f78-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="48f78-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="48f78-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48f78-131">Property</span></span>|<span data-ttu-id="48f78-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="48f78-132">Type</span></span>|<span data-ttu-id="48f78-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="48f78-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48f78-134">appProvisioningConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="48f78-134">appProvisioningConfigurationGroupAssignments</span></span>|<span data-ttu-id="48f78-135">coleção [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="48f78-135">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="48f78-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48f78-136">Not yet documented</span></span>|
|<span data-ttu-id="48f78-137">iOSLobAppProvisioningConfigAssignments</span><span class="sxs-lookup"><span data-stu-id="48f78-137">iOSLobAppProvisioningConfigAssignments</span></span>|<span data-ttu-id="48f78-138">coleção [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="48f78-138">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="48f78-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48f78-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="48f78-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="48f78-140">Response</span></span>
<span data-ttu-id="48f78-141">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="48f78-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="48f78-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48f78-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="48f78-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48f78-143">Request</span></span>
<span data-ttu-id="48f78-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48f78-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign

Content-type: application/json
Content-length: 578

{
  "appProvisioningConfigurationGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
      "targetGroupId": "Target Group Id value",
      "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
    }
  ],
  "iOSLobAppProvisioningConfigAssignments": [
    {
      "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
      "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="48f78-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="48f78-145">Response</span></span>
<span data-ttu-id="48f78-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48f78-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









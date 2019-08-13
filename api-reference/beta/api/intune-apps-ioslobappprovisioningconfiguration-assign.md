---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e9b953caadb52f2825f128378dc3dfe8029a5352
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330843"
---
# <a name="assign-action"></a><span data-ttu-id="7110f-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="7110f-103">assign action</span></span>

> <span data-ttu-id="7110f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7110f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7110f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7110f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7110f-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7110f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7110f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7110f-107">Prerequisites</span></span>
<span data-ttu-id="7110f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7110f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7110f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7110f-110">Permission type</span></span>|<span data-ttu-id="7110f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7110f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7110f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7110f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7110f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7110f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7110f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7110f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7110f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7110f-115">Not supported.</span></span>|
|<span data-ttu-id="7110f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7110f-116">Application</span></span>|<span data-ttu-id="7110f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7110f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7110f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7110f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="7110f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7110f-119">Request headers</span></span>
|<span data-ttu-id="7110f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7110f-120">Header</span></span>|<span data-ttu-id="7110f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7110f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7110f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7110f-122">Authorization</span></span>|<span data-ttu-id="7110f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7110f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7110f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7110f-124">Accept</span></span>|<span data-ttu-id="7110f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7110f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7110f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7110f-126">Request body</span></span>
<span data-ttu-id="7110f-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7110f-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7110f-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="7110f-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7110f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7110f-129">Property</span></span>|<span data-ttu-id="7110f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7110f-130">Type</span></span>|<span data-ttu-id="7110f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7110f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7110f-132">appProvisioningConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="7110f-132">appProvisioningConfigurationGroupAssignments</span></span>|<span data-ttu-id="7110f-133">coleção [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7110f-133">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="7110f-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7110f-134">Not yet documented</span></span>|
|<span data-ttu-id="7110f-135">iOSLobAppProvisioningConfigAssignments</span><span class="sxs-lookup"><span data-stu-id="7110f-135">iOSLobAppProvisioningConfigAssignments</span></span>|<span data-ttu-id="7110f-136">coleção [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7110f-136">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="7110f-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7110f-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7110f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7110f-138">Response</span></span>
<span data-ttu-id="7110f-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7110f-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7110f-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7110f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="7110f-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7110f-141">Request</span></span>
<span data-ttu-id="7110f-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7110f-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7110f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7110f-143">Response</span></span>
<span data-ttu-id="7110f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7110f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







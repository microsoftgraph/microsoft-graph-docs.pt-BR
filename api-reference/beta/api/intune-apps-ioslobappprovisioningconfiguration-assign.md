---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0a5e70fb51e45b0b753016835ffd1a9f75f57ca0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951901"
---
# <a name="assign-action"></a><span data-ttu-id="9bf09-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="9bf09-103">assign action</span></span>

> <span data-ttu-id="9bf09-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9bf09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bf09-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9bf09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bf09-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9bf09-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bf09-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9bf09-107">Prerequisites</span></span>
<span data-ttu-id="9bf09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bf09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bf09-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bf09-110">Permission type</span></span>|<span data-ttu-id="9bf09-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9bf09-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bf09-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bf09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9bf09-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bf09-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9bf09-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bf09-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bf09-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bf09-115">Not supported.</span></span>|
|<span data-ttu-id="9bf09-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bf09-116">Application</span></span>|<span data-ttu-id="9bf09-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bf09-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bf09-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bf09-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="9bf09-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf09-119">Request headers</span></span>
|<span data-ttu-id="9bf09-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9bf09-120">Header</span></span>|<span data-ttu-id="9bf09-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9bf09-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bf09-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bf09-122">Authorization</span></span>|<span data-ttu-id="9bf09-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bf09-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bf09-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9bf09-124">Accept</span></span>|<span data-ttu-id="9bf09-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9bf09-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bf09-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf09-126">Request body</span></span>
<span data-ttu-id="9bf09-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9bf09-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9bf09-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="9bf09-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9bf09-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bf09-129">Property</span></span>|<span data-ttu-id="9bf09-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bf09-130">Type</span></span>|<span data-ttu-id="9bf09-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bf09-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bf09-132">appProvisioningConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="9bf09-132">appProvisioningConfigurationGroupAssignments</span></span>|<span data-ttu-id="9bf09-133">coleção [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9bf09-133">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="9bf09-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9bf09-134">Not yet documented</span></span>|
|<span data-ttu-id="9bf09-135">iOSLobAppProvisioningConfigAssignments</span><span class="sxs-lookup"><span data-stu-id="9bf09-135">iOSLobAppProvisioningConfigAssignments</span></span>|<span data-ttu-id="9bf09-136">coleção [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9bf09-136">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="9bf09-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9bf09-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9bf09-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bf09-138">Response</span></span>
<span data-ttu-id="9bf09-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9bf09-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9bf09-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bf09-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bf09-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf09-141">Request</span></span>
<span data-ttu-id="9bf09-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bf09-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9bf09-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bf09-143">Response</span></span>
<span data-ttu-id="9bf09-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bf09-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






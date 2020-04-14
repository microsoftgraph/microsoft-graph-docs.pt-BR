---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e265cfdb3b970deecfb5e6a92bf2b271e6106245
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453863"
---
# <a name="assign-action"></a><span data-ttu-id="3405c-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="3405c-103">assign action</span></span>

<span data-ttu-id="3405c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3405c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3405c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3405c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3405c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3405c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3405c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3405c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3405c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3405c-108">Prerequisites</span></span>
<span data-ttu-id="3405c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3405c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3405c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3405c-111">Permission type</span></span>|<span data-ttu-id="3405c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3405c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3405c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3405c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3405c-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="3405c-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="3405c-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3405c-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3405c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3405c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3405c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3405c-117">Not supported.</span></span>|
|<span data-ttu-id="3405c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3405c-118">Application</span></span>||
| <span data-ttu-id="3405c-119">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="3405c-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="3405c-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3405c-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3405c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3405c-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="3405c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3405c-122">Request headers</span></span>
|<span data-ttu-id="3405c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3405c-123">Header</span></span>|<span data-ttu-id="3405c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3405c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3405c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3405c-125">Authorization</span></span>|<span data-ttu-id="3405c-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3405c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3405c-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3405c-127">Accept</span></span>|<span data-ttu-id="3405c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3405c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3405c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3405c-129">Request body</span></span>
<span data-ttu-id="3405c-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3405c-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3405c-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3405c-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3405c-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3405c-132">Property</span></span>|<span data-ttu-id="3405c-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="3405c-133">Type</span></span>|<span data-ttu-id="3405c-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="3405c-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3405c-135">appProvisioningConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="3405c-135">appProvisioningConfigurationGroupAssignments</span></span>|<span data-ttu-id="3405c-136">coleção [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3405c-136">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="3405c-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3405c-137">Not yet documented</span></span>|
|<span data-ttu-id="3405c-138">iOSLobAppProvisioningConfigAssignments</span><span class="sxs-lookup"><span data-stu-id="3405c-138">iOSLobAppProvisioningConfigAssignments</span></span>|<span data-ttu-id="3405c-139">coleção [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3405c-139">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3405c-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3405c-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3405c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3405c-141">Response</span></span>
<span data-ttu-id="3405c-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3405c-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3405c-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3405c-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="3405c-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3405c-144">Request</span></span>
<span data-ttu-id="3405c-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3405c-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3405c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3405c-146">Response</span></span>
<span data-ttu-id="3405c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3405c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







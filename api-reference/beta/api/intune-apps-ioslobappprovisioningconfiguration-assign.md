---
title: atribuir ação
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1e223bba105bf8e5e671272ed458b1b5c38948a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424907"
---
# <a name="assign-action"></a><span data-ttu-id="2ed5d-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="2ed5d-103">assign action</span></span>

> <span data-ttu-id="2ed5d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2ed5d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2ed5d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2ed5d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ed5d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2ed5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ed5d-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2ed5d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ed5d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ed5d-108">Prerequisites</span></span>
<span data-ttu-id="2ed5d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2ed5d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2ed5d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ed5d-111">Permission type</span></span>|<span data-ttu-id="2ed5d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ed5d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ed5d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ed5d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ed5d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ed5d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2ed5d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ed5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ed5d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ed5d-116">Not supported.</span></span>|
|<span data-ttu-id="2ed5d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ed5d-117">Application</span></span>|<span data-ttu-id="2ed5d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ed5d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ed5d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ed5d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="2ed5d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ed5d-120">Request headers</span></span>
|<span data-ttu-id="2ed5d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ed5d-121">Header</span></span>|<span data-ttu-id="2ed5d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2ed5d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ed5d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ed5d-123">Authorization</span></span>|<span data-ttu-id="2ed5d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ed5d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ed5d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ed5d-125">Accept</span></span>|<span data-ttu-id="2ed5d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ed5d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ed5d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ed5d-127">Request body</span></span>
<span data-ttu-id="2ed5d-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="2ed5d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2ed5d-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="2ed5d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2ed5d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ed5d-130">Property</span></span>|<span data-ttu-id="2ed5d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ed5d-131">Type</span></span>|<span data-ttu-id="2ed5d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ed5d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ed5d-133">appProvisioningConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="2ed5d-133">appProvisioningConfigurationGroupAssignments</span></span>|<span data-ttu-id="2ed5d-134">coleção [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2ed5d-134">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="2ed5d-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2ed5d-135">Not yet documented</span></span>|
|<span data-ttu-id="2ed5d-136">iOSLobAppProvisioningConfigAssignments</span><span class="sxs-lookup"><span data-stu-id="2ed5d-136">iOSLobAppProvisioningConfigAssignments</span></span>|<span data-ttu-id="2ed5d-137">coleção [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2ed5d-137">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2ed5d-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2ed5d-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2ed5d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ed5d-139">Response</span></span>
<span data-ttu-id="2ed5d-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2ed5d-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2ed5d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ed5d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ed5d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ed5d-142">Request</span></span>
<span data-ttu-id="2ed5d-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ed5d-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2ed5d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ed5d-144">Response</span></span>
<span data-ttu-id="2ed5d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ed5d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 540037998280858e50cf1ee6a9996664ff45d1c3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836971"
---
# <a name="assign-action"></a><span data-ttu-id="b1ec7-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="b1ec7-103">assign action</span></span>

> <span data-ttu-id="b1ec7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b1ec7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1ec7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b1ec7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1ec7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b1ec7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1ec7-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1ec7-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b1ec7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b1ec7-108">Prerequisites</span></span>
<span data-ttu-id="b1ec7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1ec7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1ec7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1ec7-111">Permission type</span></span>|<span data-ttu-id="b1ec7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b1ec7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1ec7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1ec7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1ec7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1ec7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1ec7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1ec7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1ec7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1ec7-116">Not supported.</span></span>|
|<span data-ttu-id="b1ec7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1ec7-117">Application</span></span>|<span data-ttu-id="b1ec7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1ec7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1ec7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1ec7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="b1ec7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1ec7-120">Request headers</span></span>
|<span data-ttu-id="b1ec7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1ec7-121">Header</span></span>|<span data-ttu-id="b1ec7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b1ec7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1ec7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1ec7-123">Authorization</span></span>|<span data-ttu-id="b1ec7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1ec7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1ec7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b1ec7-125">Accept</span></span>|<span data-ttu-id="b1ec7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1ec7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1ec7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1ec7-127">Request body</span></span>
<span data-ttu-id="b1ec7-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b1ec7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b1ec7-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b1ec7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b1ec7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1ec7-130">Property</span></span>|<span data-ttu-id="b1ec7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1ec7-131">Type</span></span>|<span data-ttu-id="b1ec7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1ec7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1ec7-133">deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="b1ec7-133">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="b1ec7-134">coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b1ec7-134">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="b1ec7-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1ec7-135">Not yet documented</span></span>|
|<span data-ttu-id="b1ec7-136">assignments</span><span class="sxs-lookup"><span data-stu-id="b1ec7-136">assignments</span></span>|<span data-ttu-id="b1ec7-137">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b1ec7-137">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b1ec7-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1ec7-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b1ec7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1ec7-139">Response</span></span>
<span data-ttu-id="b1ec7-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1ec7-140">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1ec7-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1ec7-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b1ec7-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1ec7-142">Request</span></span>
<span data-ttu-id="b1ec7-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1ec7-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 548

{
  "deviceConfigurationGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ],
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b1ec7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1ec7-144">Response</span></span>
<span data-ttu-id="b1ec7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1ec7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```






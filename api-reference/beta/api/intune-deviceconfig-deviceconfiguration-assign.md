---
title: atribuir ação
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5d30818be0733d7b571f0c2e32fb01af5570d65
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400330"
---
# <a name="assign-action"></a><span data-ttu-id="767d1-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="767d1-103">assign action</span></span>

> <span data-ttu-id="767d1-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="767d1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="767d1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="767d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="767d1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="767d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="767d1-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="767d1-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="767d1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="767d1-108">Prerequisites</span></span>
<span data-ttu-id="767d1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="767d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="767d1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="767d1-111">Permission type</span></span>|<span data-ttu-id="767d1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="767d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="767d1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="767d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="767d1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="767d1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="767d1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="767d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="767d1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="767d1-116">Not supported.</span></span>|
|<span data-ttu-id="767d1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="767d1-117">Application</span></span>|<span data-ttu-id="767d1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="767d1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="767d1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="767d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="767d1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="767d1-120">Request headers</span></span>
|<span data-ttu-id="767d1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="767d1-121">Header</span></span>|<span data-ttu-id="767d1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="767d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="767d1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="767d1-123">Authorization</span></span>|<span data-ttu-id="767d1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="767d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="767d1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="767d1-125">Accept</span></span>|<span data-ttu-id="767d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="767d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="767d1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="767d1-127">Request body</span></span>
<span data-ttu-id="767d1-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="767d1-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="767d1-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="767d1-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="767d1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="767d1-130">Property</span></span>|<span data-ttu-id="767d1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="767d1-131">Type</span></span>|<span data-ttu-id="767d1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="767d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="767d1-133">deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="767d1-133">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="767d1-134">coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="767d1-134">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="767d1-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="767d1-135">Not yet documented</span></span>|
|<span data-ttu-id="767d1-136">assignments</span><span class="sxs-lookup"><span data-stu-id="767d1-136">assignments</span></span>|<span data-ttu-id="767d1-137">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="767d1-137">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="767d1-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="767d1-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="767d1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="767d1-139">Response</span></span>
<span data-ttu-id="767d1-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="767d1-140">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="767d1-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="767d1-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="767d1-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="767d1-142">Request</span></span>
<span data-ttu-id="767d1-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="767d1-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="767d1-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="767d1-144">Response</span></span>
<span data-ttu-id="767d1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="767d1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





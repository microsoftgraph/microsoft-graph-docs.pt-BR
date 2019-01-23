---
title: Atualizar mobileAppProvisioningConfigGroupAssignment
description: Atualize as propriedades de um objeto mobileAppProvisioningConfigGroupAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b897e377ef221cc14034dbd48958a2092dbf956
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413427"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="dae1f-103">Atualizar mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="dae1f-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="dae1f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="dae1f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dae1f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dae1f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dae1f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="dae1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dae1f-107">Atualize as propriedades de um objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="dae1f-107">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dae1f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dae1f-108">Prerequisites</span></span>
<span data-ttu-id="dae1f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dae1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dae1f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dae1f-111">Permission type</span></span>|<span data-ttu-id="dae1f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dae1f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dae1f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dae1f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dae1f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dae1f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dae1f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dae1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dae1f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dae1f-116">Not supported.</span></span>|
|<span data-ttu-id="dae1f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dae1f-117">Application</span></span>|<span data-ttu-id="dae1f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dae1f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dae1f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dae1f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="dae1f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dae1f-120">Request headers</span></span>
|<span data-ttu-id="dae1f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dae1f-121">Header</span></span>|<span data-ttu-id="dae1f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dae1f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dae1f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dae1f-123">Authorization</span></span>|<span data-ttu-id="dae1f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dae1f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dae1f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dae1f-125">Accept</span></span>|<span data-ttu-id="dae1f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dae1f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dae1f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dae1f-127">Request body</span></span>
<span data-ttu-id="dae1f-128">No corpo da solicitação, fornece uma representação JSON para o objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="dae1f-128">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="dae1f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dae1f-129">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="dae1f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dae1f-130">Property</span></span>|<span data-ttu-id="dae1f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dae1f-131">Type</span></span>|<span data-ttu-id="dae1f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dae1f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dae1f-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="dae1f-133">targetGroupId</span></span>|<span data-ttu-id="dae1f-134">String</span><span class="sxs-lookup"><span data-stu-id="dae1f-134">String</span></span>|<span data-ttu-id="dae1f-135">A identificação do grupo AAD no qual o provisionamento de configuração de aplicativo está sendo direcionado.</span><span class="sxs-lookup"><span data-stu-id="dae1f-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="dae1f-136">id</span><span class="sxs-lookup"><span data-stu-id="dae1f-136">id</span></span>|<span data-ttu-id="dae1f-137">String</span><span class="sxs-lookup"><span data-stu-id="dae1f-137">String</span></span>|<span data-ttu-id="dae1f-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dae1f-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="dae1f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="dae1f-139">Response</span></span>
<span data-ttu-id="dae1f-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dae1f-140">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dae1f-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dae1f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="dae1f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dae1f-142">Request</span></span>
<span data-ttu-id="dae1f-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dae1f-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="dae1f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="dae1f-144">Response</span></span>
<span data-ttu-id="dae1f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dae1f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```





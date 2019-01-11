---
title: Atualizar mobileAppProvisioningConfigGroupAssignment
description: Atualize as propriedades de um objeto mobileAppProvisioningConfigGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b341de06c1bd5d504e4835ebef8fce2aa3a5aac7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848339"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="b54df-103">Atualizar mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b54df-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="b54df-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b54df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b54df-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b54df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b54df-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b54df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b54df-107">Atualize as propriedades de um objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b54df-107">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b54df-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b54df-108">Prerequisites</span></span>
<span data-ttu-id="b54df-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b54df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b54df-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b54df-111">Permission type</span></span>|<span data-ttu-id="b54df-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b54df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b54df-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b54df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b54df-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b54df-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b54df-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b54df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b54df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b54df-116">Not supported.</span></span>|
|<span data-ttu-id="b54df-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b54df-117">Application</span></span>|<span data-ttu-id="b54df-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b54df-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b54df-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b54df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b54df-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b54df-120">Request headers</span></span>
|<span data-ttu-id="b54df-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b54df-121">Header</span></span>|<span data-ttu-id="b54df-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b54df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b54df-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b54df-123">Authorization</span></span>|<span data-ttu-id="b54df-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b54df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b54df-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b54df-125">Accept</span></span>|<span data-ttu-id="b54df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b54df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b54df-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b54df-127">Request body</span></span>
<span data-ttu-id="b54df-128">No corpo da solicitação, fornece uma representação JSON para o objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b54df-128">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="b54df-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b54df-129">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="b54df-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b54df-130">Property</span></span>|<span data-ttu-id="b54df-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b54df-131">Type</span></span>|<span data-ttu-id="b54df-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b54df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b54df-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="b54df-133">targetGroupId</span></span>|<span data-ttu-id="b54df-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b54df-134">String</span></span>|<span data-ttu-id="b54df-135">A identificação do grupo AAD no qual o provisionamento de configuração de aplicativo está sendo direcionado.</span><span class="sxs-lookup"><span data-stu-id="b54df-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="b54df-136">id</span><span class="sxs-lookup"><span data-stu-id="b54df-136">id</span></span>|<span data-ttu-id="b54df-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b54df-137">String</span></span>|<span data-ttu-id="b54df-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b54df-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b54df-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b54df-139">Response</span></span>
<span data-ttu-id="b54df-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b54df-140">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b54df-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b54df-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b54df-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b54df-142">Request</span></span>
<span data-ttu-id="b54df-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b54df-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 48

{
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="b54df-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b54df-144">Response</span></span>
<span data-ttu-id="b54df-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b54df-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






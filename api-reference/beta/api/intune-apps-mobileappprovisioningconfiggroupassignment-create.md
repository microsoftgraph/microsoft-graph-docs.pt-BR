---
title: Criar mobileAppProvisioningConfigGroupAssignment
description: Crie um novo objeto de mobileAppProvisioningConfigGroupAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 50b93e4858a7f986f5ebd25e8d2b09e204bae986
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417431"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="36262-103">Criar mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="36262-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="36262-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="36262-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="36262-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="36262-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36262-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="36262-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36262-107">Crie um novo objeto de [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="36262-107">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36262-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="36262-108">Prerequisites</span></span>
<span data-ttu-id="36262-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="36262-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="36262-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36262-111">Permission type</span></span>|<span data-ttu-id="36262-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="36262-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36262-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36262-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36262-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36262-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="36262-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36262-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36262-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36262-116">Not supported.</span></span>|
|<span data-ttu-id="36262-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36262-117">Application</span></span>|<span data-ttu-id="36262-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36262-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36262-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36262-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="36262-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36262-120">Request headers</span></span>
|<span data-ttu-id="36262-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36262-121">Header</span></span>|<span data-ttu-id="36262-122">Valor</span><span class="sxs-lookup"><span data-stu-id="36262-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36262-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="36262-123">Authorization</span></span>|<span data-ttu-id="36262-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36262-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36262-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="36262-125">Accept</span></span>|<span data-ttu-id="36262-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36262-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36262-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36262-127">Request body</span></span>
<span data-ttu-id="36262-128">No corpo da solicitação, fornece uma representação JSON para o objeto mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="36262-128">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="36262-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="36262-129">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="36262-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36262-130">Property</span></span>|<span data-ttu-id="36262-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="36262-131">Type</span></span>|<span data-ttu-id="36262-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="36262-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36262-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="36262-133">targetGroupId</span></span>|<span data-ttu-id="36262-134">String</span><span class="sxs-lookup"><span data-stu-id="36262-134">String</span></span>|<span data-ttu-id="36262-135">A identificação do grupo AAD no qual o provisionamento de configuração de aplicativo está sendo direcionado.</span><span class="sxs-lookup"><span data-stu-id="36262-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="36262-136">id</span><span class="sxs-lookup"><span data-stu-id="36262-136">id</span></span>|<span data-ttu-id="36262-137">String</span><span class="sxs-lookup"><span data-stu-id="36262-137">String</span></span>|<span data-ttu-id="36262-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="36262-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="36262-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="36262-139">Response</span></span>
<span data-ttu-id="36262-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36262-140">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36262-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36262-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="36262-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36262-142">Request</span></span>
<span data-ttu-id="36262-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36262-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="36262-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="36262-144">Response</span></span>
<span data-ttu-id="36262-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36262-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```





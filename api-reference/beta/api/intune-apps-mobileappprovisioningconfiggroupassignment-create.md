---
title: Criar mobileAppProvisioningConfigGroupAssignment
description: Crie um novo objeto de mobileAppProvisioningConfigGroupAssignment.
ms.openlocfilehash: 7ff1377079ea47d7bb809b9b71d1033a4681d19d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040980"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="8c51d-103">Criar mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="8c51d-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="8c51d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8c51d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c51d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8c51d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c51d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8c51d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c51d-107">Crie um novo objeto de [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8c51d-107">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c51d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c51d-108">Prerequisites</span></span>
<span data-ttu-id="8c51d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c51d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c51d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c51d-111">Permission type</span></span>|<span data-ttu-id="8c51d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8c51d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c51d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c51d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c51d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c51d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c51d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c51d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c51d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c51d-116">Not supported.</span></span>|
|<span data-ttu-id="8c51d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c51d-117">Application</span></span>|<span data-ttu-id="8c51d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c51d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c51d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c51d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="8c51d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c51d-120">Request headers</span></span>
|<span data-ttu-id="8c51d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c51d-121">Header</span></span>|<span data-ttu-id="8c51d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8c51d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c51d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c51d-123">Authorization</span></span>|<span data-ttu-id="8c51d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c51d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c51d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8c51d-125">Accept</span></span>|<span data-ttu-id="8c51d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c51d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c51d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c51d-127">Request body</span></span>
<span data-ttu-id="8c51d-128">No corpo da solicitação, fornece uma representação JSON para o objeto mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="8c51d-128">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="8c51d-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="8c51d-129">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="8c51d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c51d-130">Property</span></span>|<span data-ttu-id="8c51d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c51d-131">Type</span></span>|<span data-ttu-id="8c51d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c51d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c51d-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="8c51d-133">targetGroupId</span></span>|<span data-ttu-id="8c51d-134">String</span><span class="sxs-lookup"><span data-stu-id="8c51d-134">String</span></span>|<span data-ttu-id="8c51d-135">A identificação do grupo AAD no qual o provisionamento de configuração de aplicativo está sendo direcionado.</span><span class="sxs-lookup"><span data-stu-id="8c51d-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="8c51d-136">id</span><span class="sxs-lookup"><span data-stu-id="8c51d-136">id</span></span>|<span data-ttu-id="8c51d-137">String</span><span class="sxs-lookup"><span data-stu-id="8c51d-137">String</span></span>|<span data-ttu-id="8c51d-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8c51d-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="8c51d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c51d-139">Response</span></span>
<span data-ttu-id="8c51d-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c51d-140">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c51d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c51d-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c51d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c51d-142">Request</span></span>
<span data-ttu-id="8c51d-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c51d-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="8c51d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c51d-144">Response</span></span>
<span data-ttu-id="8c51d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c51d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






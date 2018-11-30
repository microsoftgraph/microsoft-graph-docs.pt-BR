---
title: Criar iosLobAppProvisioningConfigurationAssignment
description: Crie um novo objeto de iosLobAppProvisioningConfigurationAssignment.
ms.openlocfilehash: 5d3a51aab8560e4922d74e48675aa95c25be5c72
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033586"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="098b0-103">Criar iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="098b0-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="098b0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="098b0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="098b0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="098b0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="098b0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="098b0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="098b0-107">Crie um novo objeto de [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="098b0-107">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="098b0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="098b0-108">Prerequisites</span></span>
<span data-ttu-id="098b0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="098b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="098b0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="098b0-111">Permission type</span></span>|<span data-ttu-id="098b0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="098b0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="098b0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="098b0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="098b0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="098b0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="098b0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="098b0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="098b0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="098b0-116">Not supported.</span></span>|
|<span data-ttu-id="098b0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="098b0-117">Application</span></span>|<span data-ttu-id="098b0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="098b0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="098b0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="098b0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="098b0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="098b0-120">Request headers</span></span>
|<span data-ttu-id="098b0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="098b0-121">Header</span></span>|<span data-ttu-id="098b0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="098b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="098b0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="098b0-123">Authorization</span></span>|<span data-ttu-id="098b0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="098b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="098b0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="098b0-125">Accept</span></span>|<span data-ttu-id="098b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="098b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="098b0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="098b0-127">Request body</span></span>
<span data-ttu-id="098b0-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="098b0-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="098b0-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="098b0-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="098b0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="098b0-130">Property</span></span>|<span data-ttu-id="098b0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="098b0-131">Type</span></span>|<span data-ttu-id="098b0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="098b0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="098b0-133">id</span><span class="sxs-lookup"><span data-stu-id="098b0-133">id</span></span>|<span data-ttu-id="098b0-134">String</span><span class="sxs-lookup"><span data-stu-id="098b0-134">String</span></span>|<span data-ttu-id="098b0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="098b0-135">Key of the entity.</span></span>|
|<span data-ttu-id="098b0-136">destino</span><span class="sxs-lookup"><span data-stu-id="098b0-136">target</span></span>|[<span data-ttu-id="098b0-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="098b0-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="098b0-138">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="098b0-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="098b0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="098b0-139">Response</span></span>
<span data-ttu-id="098b0-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="098b0-140">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="098b0-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="098b0-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="098b0-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="098b0-142">Request</span></span>
<span data-ttu-id="098b0-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="098b0-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="098b0-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="098b0-144">Response</span></span>
<span data-ttu-id="098b0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="098b0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```






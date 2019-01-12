---
title: Criar iosLobAppProvisioningConfigurationAssignment
description: Crie um novo objeto de iosLobAppProvisioningConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3e2138480d97047e7aa396becb24abb88feb4022
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925648"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="f5919-103">Criar iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f5919-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="f5919-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f5919-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5919-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f5919-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5919-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f5919-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5919-107">Crie um novo objeto de [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="f5919-107">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f5919-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5919-108">Prerequisites</span></span>
<span data-ttu-id="f5919-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5919-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5919-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5919-111">Permission type</span></span>|<span data-ttu-id="f5919-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f5919-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5919-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5919-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5919-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5919-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f5919-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5919-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5919-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5919-116">Not supported.</span></span>|
|<span data-ttu-id="f5919-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5919-117">Application</span></span>|<span data-ttu-id="f5919-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5919-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5919-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5919-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f5919-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5919-120">Request headers</span></span>
|<span data-ttu-id="f5919-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5919-121">Header</span></span>|<span data-ttu-id="f5919-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f5919-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5919-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5919-123">Authorization</span></span>|<span data-ttu-id="f5919-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5919-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5919-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5919-125">Accept</span></span>|<span data-ttu-id="f5919-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5919-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5919-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5919-127">Request body</span></span>
<span data-ttu-id="f5919-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="f5919-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="f5919-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="f5919-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="f5919-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5919-130">Property</span></span>|<span data-ttu-id="f5919-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5919-131">Type</span></span>|<span data-ttu-id="f5919-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5919-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5919-133">id</span><span class="sxs-lookup"><span data-stu-id="f5919-133">id</span></span>|<span data-ttu-id="f5919-134">String</span><span class="sxs-lookup"><span data-stu-id="f5919-134">String</span></span>|<span data-ttu-id="f5919-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f5919-135">Key of the entity.</span></span>|
|<span data-ttu-id="f5919-136">destino</span><span class="sxs-lookup"><span data-stu-id="f5919-136">target</span></span>|[<span data-ttu-id="f5919-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f5919-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f5919-138">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f5919-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="f5919-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5919-139">Response</span></span>
<span data-ttu-id="f5919-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5919-140">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5919-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5919-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="f5919-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5919-142">Request</span></span>
<span data-ttu-id="f5919-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5919-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f5919-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5919-144">Response</span></span>
<span data-ttu-id="f5919-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5919-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






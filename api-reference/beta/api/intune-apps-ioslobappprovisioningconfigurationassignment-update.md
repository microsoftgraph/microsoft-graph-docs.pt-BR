---
title: Atualizar iosLobAppProvisioningConfigurationAssignment
description: Atualize as propriedades de um objeto iosLobAppProvisioningConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aa713ab3293cfcb922d8e85306bcf2645b549450
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832575"
---
# <a name="update-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="60aad-103">Atualizar iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="60aad-103">Update iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="60aad-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="60aad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60aad-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="60aad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60aad-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="60aad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60aad-107">Atualize as propriedades de um objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="60aad-107">Update the properties of a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="60aad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60aad-108">Prerequisites</span></span>
<span data-ttu-id="60aad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60aad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60aad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60aad-111">Permission type</span></span>|<span data-ttu-id="60aad-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="60aad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60aad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60aad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60aad-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60aad-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60aad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60aad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60aad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60aad-116">Not supported.</span></span>|
|<span data-ttu-id="60aad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60aad-117">Application</span></span>|<span data-ttu-id="60aad-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60aad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60aad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60aad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="60aad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60aad-120">Request headers</span></span>
|<span data-ttu-id="60aad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60aad-121">Header</span></span>|<span data-ttu-id="60aad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="60aad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60aad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="60aad-123">Authorization</span></span>|<span data-ttu-id="60aad-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60aad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60aad-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60aad-125">Accept</span></span>|<span data-ttu-id="60aad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60aad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60aad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60aad-127">Request body</span></span>
<span data-ttu-id="60aad-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="60aad-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

<span data-ttu-id="60aad-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="60aad-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

|<span data-ttu-id="60aad-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60aad-130">Property</span></span>|<span data-ttu-id="60aad-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="60aad-131">Type</span></span>|<span data-ttu-id="60aad-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="60aad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60aad-133">id</span><span class="sxs-lookup"><span data-stu-id="60aad-133">id</span></span>|<span data-ttu-id="60aad-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60aad-134">String</span></span>|<span data-ttu-id="60aad-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="60aad-135">Key of the entity.</span></span>|
|<span data-ttu-id="60aad-136">destino</span><span class="sxs-lookup"><span data-stu-id="60aad-136">target</span></span>|[<span data-ttu-id="60aad-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="60aad-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="60aad-138">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="60aad-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="60aad-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="60aad-139">Response</span></span>
<span data-ttu-id="60aad-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60aad-140">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60aad-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60aad-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="60aad-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60aad-142">Request</span></span>
<span data-ttu-id="60aad-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60aad-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="60aad-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="60aad-144">Response</span></span>
<span data-ttu-id="60aad-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60aad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






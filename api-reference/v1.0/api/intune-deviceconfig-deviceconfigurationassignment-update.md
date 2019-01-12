---
title: Atualizar deviceConfigurationAssignment
description: Atualizar as propriedades de um objeto deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1b3e2931e791c0d7e57e3a9e47896bf1ac7c64f5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947488"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="d7278-103">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d7278-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="d7278-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d7278-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7278-105">Atualizar as propriedades de um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d7278-105">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d7278-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d7278-106">Prerequisites</span></span>
<span data-ttu-id="d7278-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7278-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7278-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7278-109">Permission type</span></span>|<span data-ttu-id="d7278-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d7278-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7278-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7278-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d7278-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7278-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7278-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7278-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7278-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7278-114">Not supported.</span></span>|
|<span data-ttu-id="d7278-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7278-115">Application</span></span>|<span data-ttu-id="d7278-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7278-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7278-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7278-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d7278-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7278-118">Request headers</span></span>
|<span data-ttu-id="d7278-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d7278-119">Header</span></span>|<span data-ttu-id="d7278-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d7278-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7278-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7278-121">Authorization</span></span>|<span data-ttu-id="d7278-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7278-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7278-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d7278-123">Accept</span></span>|<span data-ttu-id="d7278-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d7278-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7278-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7278-125">Request body</span></span>
<span data-ttu-id="d7278-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d7278-126">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="d7278-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d7278-127">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="d7278-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7278-128">Property</span></span>|<span data-ttu-id="d7278-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7278-129">Type</span></span>|<span data-ttu-id="d7278-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7278-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7278-131">id</span><span class="sxs-lookup"><span data-stu-id="d7278-131">id</span></span>|<span data-ttu-id="d7278-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7278-132">String</span></span>|<span data-ttu-id="d7278-133">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="d7278-133">The key of the assignment.</span></span>|
|<span data-ttu-id="d7278-134">destino</span><span class="sxs-lookup"><span data-stu-id="d7278-134">target</span></span>|[<span data-ttu-id="d7278-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d7278-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d7278-136">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d7278-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="d7278-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7278-137">Response</span></span>
<span data-ttu-id="d7278-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7278-138">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7278-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7278-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="d7278-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7278-140">Request</span></span>
<span data-ttu-id="d7278-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7278-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d7278-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7278-142">Response</span></span>
<span data-ttu-id="d7278-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7278-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




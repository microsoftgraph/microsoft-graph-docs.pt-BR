---
title: Atualizar deviceConfigurationAssignment
description: Atualizar as propriedades de um objeto deviceConfigurationAssignment.
author: tfitzmac
ms.openlocfilehash: 51b0269a72dbded4f8bdd157683bc321b55874d3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336474"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="07a73-103">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="07a73-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="07a73-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="07a73-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07a73-105">Atualizar as propriedades de um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="07a73-105">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="07a73-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07a73-106">Prerequisites</span></span>
<span data-ttu-id="07a73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07a73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07a73-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07a73-109">Permission type</span></span>|<span data-ttu-id="07a73-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07a73-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07a73-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07a73-111">Delegated (work or school account)</span></span>|<span data-ttu-id="07a73-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07a73-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="07a73-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07a73-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07a73-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07a73-114">Not supported.</span></span>|
|<span data-ttu-id="07a73-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07a73-115">Application</span></span>|<span data-ttu-id="07a73-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07a73-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07a73-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07a73-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="07a73-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07a73-118">Request headers</span></span>
|<span data-ttu-id="07a73-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07a73-119">Header</span></span>|<span data-ttu-id="07a73-120">Valor</span><span class="sxs-lookup"><span data-stu-id="07a73-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07a73-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="07a73-121">Authorization</span></span>|<span data-ttu-id="07a73-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07a73-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07a73-123">Accept</span><span class="sxs-lookup"><span data-stu-id="07a73-123">Accept</span></span>|<span data-ttu-id="07a73-124">application/json</span><span class="sxs-lookup"><span data-stu-id="07a73-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07a73-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07a73-125">Request body</span></span>
<span data-ttu-id="07a73-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="07a73-126">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="07a73-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="07a73-127">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="07a73-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07a73-128">Property</span></span>|<span data-ttu-id="07a73-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="07a73-129">Type</span></span>|<span data-ttu-id="07a73-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="07a73-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07a73-131">id</span><span class="sxs-lookup"><span data-stu-id="07a73-131">id</span></span>|<span data-ttu-id="07a73-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07a73-132">String</span></span>|<span data-ttu-id="07a73-133">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="07a73-133">The key of the assignment.</span></span>|
|<span data-ttu-id="07a73-134">destino</span><span class="sxs-lookup"><span data-stu-id="07a73-134">target</span></span>|[<span data-ttu-id="07a73-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="07a73-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="07a73-136">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="07a73-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="07a73-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="07a73-137">Response</span></span>
<span data-ttu-id="07a73-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07a73-138">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07a73-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07a73-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="07a73-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07a73-140">Request</span></span>
<span data-ttu-id="07a73-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07a73-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="07a73-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="07a73-142">Response</span></span>
<span data-ttu-id="07a73-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07a73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




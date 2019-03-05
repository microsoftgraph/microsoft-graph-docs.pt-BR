---
title: Atualizar deviceConfigurationAssignment
description: Atualizar as propriedades de um objeto deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c76a7ae809f0445a445f51c5e5dd270614b518d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250744"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="45a08-103">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="45a08-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="45a08-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45a08-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45a08-105">Atualizar as propriedades de um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="45a08-105">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45a08-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45a08-106">Prerequisites</span></span>
<span data-ttu-id="45a08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="45a08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="45a08-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45a08-109">Permission type</span></span>|<span data-ttu-id="45a08-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45a08-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45a08-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45a08-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45a08-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45a08-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45a08-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45a08-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45a08-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45a08-114">Not supported.</span></span>|
|<span data-ttu-id="45a08-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45a08-115">Application</span></span>|<span data-ttu-id="45a08-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45a08-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45a08-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45a08-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="45a08-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45a08-118">Request headers</span></span>
|<span data-ttu-id="45a08-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45a08-119">Header</span></span>|<span data-ttu-id="45a08-120">Valor</span><span class="sxs-lookup"><span data-stu-id="45a08-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45a08-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="45a08-121">Authorization</span></span>|<span data-ttu-id="45a08-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45a08-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45a08-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45a08-123">Accept</span></span>|<span data-ttu-id="45a08-124">application/json</span><span class="sxs-lookup"><span data-stu-id="45a08-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45a08-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45a08-125">Request body</span></span>
<span data-ttu-id="45a08-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="45a08-126">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="45a08-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="45a08-127">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="45a08-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45a08-128">Property</span></span>|<span data-ttu-id="45a08-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="45a08-129">Type</span></span>|<span data-ttu-id="45a08-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="45a08-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45a08-131">id</span><span class="sxs-lookup"><span data-stu-id="45a08-131">id</span></span>|<span data-ttu-id="45a08-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45a08-132">String</span></span>|<span data-ttu-id="45a08-133">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="45a08-133">The key of the assignment.</span></span>|
|<span data-ttu-id="45a08-134">destino</span><span class="sxs-lookup"><span data-stu-id="45a08-134">target</span></span>|[<span data-ttu-id="45a08-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="45a08-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="45a08-136">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45a08-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="45a08-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="45a08-137">Response</span></span>
<span data-ttu-id="45a08-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45a08-138">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45a08-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45a08-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="45a08-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45a08-140">Request</span></span>
<span data-ttu-id="45a08-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45a08-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="45a08-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="45a08-142">Response</span></span>
<span data-ttu-id="45a08-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45a08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




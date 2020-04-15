---
title: Atualizar deviceConfigurationAssignment
description: Atualizar as propriedades de um objeto deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dc8ce69735094496174dab83639a32f3a2c16df8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43370495"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="7baef-103">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7baef-103">Update deviceConfigurationAssignment</span></span>

<span data-ttu-id="7baef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7baef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7baef-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7baef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7baef-106">Atualizar as propriedades de um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7baef-106">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7baef-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7baef-107">Prerequisites</span></span>
<span data-ttu-id="7baef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7baef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7baef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7baef-110">Permission type</span></span>|<span data-ttu-id="7baef-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7baef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7baef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7baef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7baef-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7baef-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7baef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7baef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7baef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7baef-115">Not supported.</span></span>|
|<span data-ttu-id="7baef-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7baef-116">Application</span></span>|<span data-ttu-id="7baef-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7baef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7baef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7baef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7baef-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7baef-119">Request headers</span></span>
|<span data-ttu-id="7baef-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7baef-120">Header</span></span>|<span data-ttu-id="7baef-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7baef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7baef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7baef-122">Authorization</span></span>|<span data-ttu-id="7baef-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7baef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7baef-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7baef-124">Accept</span></span>|<span data-ttu-id="7baef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7baef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7baef-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7baef-126">Request body</span></span>
<span data-ttu-id="7baef-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7baef-127">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="7baef-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7baef-128">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="7baef-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7baef-129">Property</span></span>|<span data-ttu-id="7baef-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7baef-130">Type</span></span>|<span data-ttu-id="7baef-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7baef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7baef-132">id</span><span class="sxs-lookup"><span data-stu-id="7baef-132">id</span></span>|<span data-ttu-id="7baef-133">String</span><span class="sxs-lookup"><span data-stu-id="7baef-133">String</span></span>|<span data-ttu-id="7baef-134">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="7baef-134">The key of the assignment.</span></span>|
|<span data-ttu-id="7baef-135">destino</span><span class="sxs-lookup"><span data-stu-id="7baef-135">target</span></span>|[<span data-ttu-id="7baef-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7baef-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7baef-137">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7baef-137">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="7baef-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7baef-138">Response</span></span>
<span data-ttu-id="7baef-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7baef-139">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7baef-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7baef-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="7baef-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7baef-141">Request</span></span>
<span data-ttu-id="7baef-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7baef-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7baef-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7baef-143">Response</span></span>
<span data-ttu-id="7baef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7baef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







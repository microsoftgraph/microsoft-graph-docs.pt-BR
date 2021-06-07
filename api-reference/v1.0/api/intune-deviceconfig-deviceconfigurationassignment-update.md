---
title: Atualizar deviceConfigurationAssignment
description: Atualizar as propriedades de um objeto deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a74c2fe13a60a1184b8cd36b6e353c59dce88ce6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748373"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="642b5-103">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="642b5-103">Update deviceConfigurationAssignment</span></span>

<span data-ttu-id="642b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="642b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="642b5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="642b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="642b5-106">Atualizar as propriedades de um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="642b5-106">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="642b5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="642b5-107">Prerequisites</span></span>
<span data-ttu-id="642b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="642b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="642b5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="642b5-110">Permission type</span></span>|<span data-ttu-id="642b5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="642b5-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="642b5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="642b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="642b5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="642b5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="642b5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="642b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="642b5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="642b5-115">Not supported.</span></span>|
|<span data-ttu-id="642b5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="642b5-116">Application</span></span>|<span data-ttu-id="642b5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="642b5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="642b5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="642b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="642b5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="642b5-119">Request headers</span></span>
|<span data-ttu-id="642b5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="642b5-120">Header</span></span>|<span data-ttu-id="642b5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="642b5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="642b5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="642b5-122">Authorization</span></span>|<span data-ttu-id="642b5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="642b5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="642b5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="642b5-124">Accept</span></span>|<span data-ttu-id="642b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="642b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="642b5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="642b5-126">Request body</span></span>
<span data-ttu-id="642b5-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="642b5-127">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="642b5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="642b5-128">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="642b5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="642b5-129">Property</span></span>|<span data-ttu-id="642b5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="642b5-130">Type</span></span>|<span data-ttu-id="642b5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="642b5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="642b5-132">id</span><span class="sxs-lookup"><span data-stu-id="642b5-132">id</span></span>|<span data-ttu-id="642b5-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="642b5-133">String</span></span>|<span data-ttu-id="642b5-134">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="642b5-134">The key of the assignment.</span></span>|
|<span data-ttu-id="642b5-135">destino</span><span class="sxs-lookup"><span data-stu-id="642b5-135">target</span></span>|[<span data-ttu-id="642b5-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="642b5-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="642b5-137">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="642b5-137">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="642b5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="642b5-138">Response</span></span>
<span data-ttu-id="642b5-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="642b5-139">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="642b5-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="642b5-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="642b5-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="642b5-141">Request</span></span>
<span data-ttu-id="642b5-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="642b5-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 221

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="642b5-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="642b5-143">Response</span></span>
<span data-ttu-id="642b5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="642b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "collectionId": "Collection Id value"
  }
}
```





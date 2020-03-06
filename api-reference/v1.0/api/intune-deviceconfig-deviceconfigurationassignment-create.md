---
title: Criar deviceConfigurationAssignment
description: Criar um novo objeto deviceConfigurationAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 28d695fd5e0e02bbb4f32fdf703b4c8ba96f38b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514835"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="ebe45-103">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ebe45-103">Create deviceConfigurationAssignment</span></span>

<span data-ttu-id="ebe45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebe45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebe45-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebe45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebe45-106">Criar um novo objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ebe45-106">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebe45-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ebe45-107">Prerequisites</span></span>
<span data-ttu-id="ebe45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebe45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebe45-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebe45-110">Permission type</span></span>|<span data-ttu-id="ebe45-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ebe45-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebe45-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebe45-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ebe45-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebe45-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ebe45-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebe45-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebe45-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebe45-115">Not supported.</span></span>|
|<span data-ttu-id="ebe45-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebe45-116">Application</span></span>|<span data-ttu-id="ebe45-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebe45-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebe45-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebe45-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ebe45-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebe45-119">Request headers</span></span>
|<span data-ttu-id="ebe45-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebe45-120">Header</span></span>|<span data-ttu-id="ebe45-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ebe45-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebe45-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebe45-122">Authorization</span></span>|<span data-ttu-id="ebe45-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebe45-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebe45-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ebe45-124">Accept</span></span>|<span data-ttu-id="ebe45-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ebe45-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebe45-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebe45-126">Request body</span></span>
<span data-ttu-id="ebe45-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="ebe45-127">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="ebe45-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="ebe45-128">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="ebe45-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebe45-129">Property</span></span>|<span data-ttu-id="ebe45-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebe45-130">Type</span></span>|<span data-ttu-id="ebe45-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebe45-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebe45-132">id</span><span class="sxs-lookup"><span data-stu-id="ebe45-132">id</span></span>|<span data-ttu-id="ebe45-133">String</span><span class="sxs-lookup"><span data-stu-id="ebe45-133">String</span></span>|<span data-ttu-id="ebe45-134">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="ebe45-134">The key of the assignment.</span></span>|
|<span data-ttu-id="ebe45-135">destino</span><span class="sxs-lookup"><span data-stu-id="ebe45-135">target</span></span>|[<span data-ttu-id="ebe45-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ebe45-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ebe45-137">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ebe45-137">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="ebe45-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebe45-138">Response</span></span>
<span data-ttu-id="ebe45-139">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebe45-139">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebe45-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebe45-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebe45-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebe45-141">Request</span></span>
<span data-ttu-id="ebe45-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebe45-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ebe45-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebe45-143">Response</span></span>
<span data-ttu-id="ebe45-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebe45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





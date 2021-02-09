---
title: Criar windowsQualityUpdateProfileAssignment
description: Crie um novo objeto windowsQualityUpdateProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 19c34d199e4ec1e46fbf3ed0ef9692bdd02da53f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160112"
---
# <a name="create-windowsqualityupdateprofileassignment"></a><span data-ttu-id="2cc79-103">Criar windowsQualityUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="2cc79-103">Create windowsQualityUpdateProfileAssignment</span></span>

<span data-ttu-id="2cc79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cc79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2cc79-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2cc79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cc79-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2cc79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cc79-107">Crie um novo [objeto windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2cc79-107">Create a new [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cc79-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2cc79-108">Prerequisites</span></span>
<span data-ttu-id="2cc79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cc79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cc79-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2cc79-111">Permission type</span></span>|<span data-ttu-id="2cc79-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2cc79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cc79-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2cc79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2cc79-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc79-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2cc79-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2cc79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cc79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2cc79-116">Not supported.</span></span>|
|<span data-ttu-id="2cc79-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2cc79-117">Application</span></span>|<span data-ttu-id="2cc79-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc79-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cc79-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2cc79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2cc79-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2cc79-120">Request headers</span></span>
|<span data-ttu-id="2cc79-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2cc79-121">Header</span></span>|<span data-ttu-id="2cc79-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2cc79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cc79-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2cc79-123">Authorization</span></span>|<span data-ttu-id="2cc79-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2cc79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cc79-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2cc79-125">Accept</span></span>|<span data-ttu-id="2cc79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2cc79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cc79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2cc79-127">Request body</span></span>
<span data-ttu-id="2cc79-128">No corpo da solicitação, fornece uma representação JSON do objeto windowsQualityUpdateProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="2cc79-128">In the request body, supply a JSON representation for the windowsQualityUpdateProfileAssignment object.</span></span>

<span data-ttu-id="2cc79-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsQualityUpdateProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="2cc79-129">The following table shows the properties that are required when you create the windowsQualityUpdateProfileAssignment.</span></span>

|<span data-ttu-id="2cc79-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2cc79-130">Property</span></span>|<span data-ttu-id="2cc79-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cc79-131">Type</span></span>|<span data-ttu-id="2cc79-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cc79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cc79-133">id</span><span class="sxs-lookup"><span data-stu-id="2cc79-133">id</span></span>|<span data-ttu-id="2cc79-134">String</span><span class="sxs-lookup"><span data-stu-id="2cc79-134">String</span></span>|<span data-ttu-id="2cc79-135">O identificador da entidade</span><span class="sxs-lookup"><span data-stu-id="2cc79-135">The Identifier of the entity</span></span>|
|<span data-ttu-id="2cc79-136">destino</span><span class="sxs-lookup"><span data-stu-id="2cc79-136">target</span></span>|[<span data-ttu-id="2cc79-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2cc79-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2cc79-138">O destino de atribuição ao que o perfil de atualização de recursos está atribuído.</span><span class="sxs-lookup"><span data-stu-id="2cc79-138">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="2cc79-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cc79-139">Response</span></span>
<span data-ttu-id="2cc79-140">Se bem-sucedido, este método retorna um código de resposta e um objeto `201 Created` [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2cc79-140">If successful, this method returns a `201 Created` response code and a [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cc79-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2cc79-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cc79-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2cc79-142">Request</span></span>
<span data-ttu-id="2cc79-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2cc79-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}/assignments
Content-type: application/json
Content-length: 344

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="2cc79-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cc79-144">Response</span></span>
<span data-ttu-id="2cc79-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2cc79-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 393

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
  "id": "0c3a8422-8422-0c3a-2284-3a0c22843a0c",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```





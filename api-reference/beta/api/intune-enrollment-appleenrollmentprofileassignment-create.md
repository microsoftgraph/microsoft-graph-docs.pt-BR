---
title: Criar appleEnrollmentProfileAssignment
description: Criar um novo objeto appleEnrollmentProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e41919f6a8e9201673b8e7a3e0175c8c9b1926ae
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944157"
---
# <a name="create-appleenrollmentprofileassignment"></a><span data-ttu-id="b95ca-103">Criar appleEnrollmentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="b95ca-103">Create appleEnrollmentProfileAssignment</span></span>

> <span data-ttu-id="b95ca-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b95ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b95ca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b95ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b95ca-106">Criar um novo objeto [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b95ca-106">Create a new [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b95ca-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b95ca-107">Prerequisites</span></span>
<span data-ttu-id="b95ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b95ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b95ca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b95ca-110">Permission type</span></span>|<span data-ttu-id="b95ca-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b95ca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b95ca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b95ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b95ca-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b95ca-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b95ca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b95ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b95ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b95ca-115">Not supported.</span></span>|
|<span data-ttu-id="b95ca-116">Application</span><span class="sxs-lookup"><span data-stu-id="b95ca-116">Application</span></span>|<span data-ttu-id="b95ca-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b95ca-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b95ca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b95ca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b95ca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b95ca-119">Request headers</span></span>
|<span data-ttu-id="b95ca-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b95ca-120">Header</span></span>|<span data-ttu-id="b95ca-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b95ca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b95ca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b95ca-122">Authorization</span></span>|<span data-ttu-id="b95ca-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b95ca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b95ca-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b95ca-124">Accept</span></span>|<span data-ttu-id="b95ca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b95ca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b95ca-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b95ca-126">Request body</span></span>
<span data-ttu-id="b95ca-127">No corpo da solicitação, forneça uma representação JSON do objeto appleEnrollmentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="b95ca-127">In the request body, supply a JSON representation for the appleEnrollmentProfileAssignment object.</span></span>

<span data-ttu-id="b95ca-128">A tabela a seguir mostra as propriedades que são necessárias ao criar appleEnrollmentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="b95ca-128">The following table shows the properties that are required when you create the appleEnrollmentProfileAssignment.</span></span>

|<span data-ttu-id="b95ca-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b95ca-129">Property</span></span>|<span data-ttu-id="b95ca-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b95ca-130">Type</span></span>|<span data-ttu-id="b95ca-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b95ca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b95ca-132">id</span><span class="sxs-lookup"><span data-stu-id="b95ca-132">id</span></span>|<span data-ttu-id="b95ca-133">String</span><span class="sxs-lookup"><span data-stu-id="b95ca-133">String</span></span>|<span data-ttu-id="b95ca-134">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="b95ca-134">The key of the assignment.</span></span>|
|<span data-ttu-id="b95ca-135">destino</span><span class="sxs-lookup"><span data-stu-id="b95ca-135">target</span></span>|[<span data-ttu-id="b95ca-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b95ca-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b95ca-137">O destino de atribuição para o perfil de implantação iniciado pelo usuário da Apple.</span><span class="sxs-lookup"><span data-stu-id="b95ca-137">The assignment target for the Apple user initiated deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="b95ca-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b95ca-138">Response</span></span>
<span data-ttu-id="b95ca-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b95ca-139">If successful, this method returns a `201 Created` response code and a [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b95ca-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b95ca-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="b95ca-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b95ca-141">Request</span></span>
<span data-ttu-id="b95ca-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b95ca-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b95ca-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b95ca-143">Response</span></span>
<span data-ttu-id="b95ca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b95ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "id": "5b603771-3771-5b60-7137-605b7137605b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```






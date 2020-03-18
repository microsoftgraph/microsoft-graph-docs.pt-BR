---
title: Criar appleEnrollmentProfileAssignment
description: Criar um novo objeto appleEnrollmentProfileAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7d28b49371f3616dd115d46756f1393425f4e96d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813527"
---
# <a name="create-appleenrollmentprofileassignment"></a><span data-ttu-id="63877-103">Criar appleEnrollmentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="63877-103">Create appleEnrollmentProfileAssignment</span></span>

> <span data-ttu-id="63877-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63877-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63877-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63877-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63877-106">Criar um novo objeto [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="63877-106">Create a new [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63877-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63877-107">Prerequisites</span></span>
<span data-ttu-id="63877-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63877-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63877-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63877-110">Permission type</span></span>|<span data-ttu-id="63877-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63877-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63877-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63877-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63877-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63877-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="63877-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63877-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63877-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63877-115">Not supported.</span></span>|
|<span data-ttu-id="63877-116">Application</span><span class="sxs-lookup"><span data-stu-id="63877-116">Application</span></span>|<span data-ttu-id="63877-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63877-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63877-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63877-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="63877-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63877-119">Request headers</span></span>
|<span data-ttu-id="63877-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63877-120">Header</span></span>|<span data-ttu-id="63877-121">Valor</span><span class="sxs-lookup"><span data-stu-id="63877-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63877-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="63877-122">Authorization</span></span>|<span data-ttu-id="63877-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63877-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63877-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63877-124">Accept</span></span>|<span data-ttu-id="63877-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63877-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63877-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63877-126">Request body</span></span>
<span data-ttu-id="63877-127">No corpo da solicitação, forneça uma representação JSON do objeto appleEnrollmentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="63877-127">In the request body, supply a JSON representation for the appleEnrollmentProfileAssignment object.</span></span>

<span data-ttu-id="63877-128">A tabela a seguir mostra as propriedades que são necessárias ao criar appleEnrollmentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="63877-128">The following table shows the properties that are required when you create the appleEnrollmentProfileAssignment.</span></span>

|<span data-ttu-id="63877-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63877-129">Property</span></span>|<span data-ttu-id="63877-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="63877-130">Type</span></span>|<span data-ttu-id="63877-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="63877-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63877-132">id</span><span class="sxs-lookup"><span data-stu-id="63877-132">id</span></span>|<span data-ttu-id="63877-133">String</span><span class="sxs-lookup"><span data-stu-id="63877-133">String</span></span>|<span data-ttu-id="63877-134">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="63877-134">The key of the assignment.</span></span>|
|<span data-ttu-id="63877-135">destino</span><span class="sxs-lookup"><span data-stu-id="63877-135">target</span></span>|[<span data-ttu-id="63877-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="63877-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="63877-137">O destino de atribuição para o perfil de implantação iniciado pelo usuário da Apple.</span><span class="sxs-lookup"><span data-stu-id="63877-137">The assignment target for the Apple user initiated deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="63877-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="63877-138">Response</span></span>
<span data-ttu-id="63877-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63877-139">If successful, this method returns a `201 Created` response code and a [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63877-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63877-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="63877-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63877-141">Request</span></span>
<span data-ttu-id="63877-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63877-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="63877-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="63877-143">Response</span></span>
<span data-ttu-id="63877-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63877-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





---
title: Criar intuneBrandingProfileAssignment
description: Crie um novo objeto de intuneBrandingProfileAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 17c6a6c1f06d383a6019c168b41187826cb63067
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429049"
---
# <a name="create-intunebrandingprofileassignment"></a><span data-ttu-id="4e30d-103">Criar intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="4e30d-103">Create intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="4e30d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4e30d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4e30d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4e30d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e30d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4e30d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e30d-107">Crie um novo objeto de [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4e30d-107">Create a new [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e30d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4e30d-108">Prerequisites</span></span>
<span data-ttu-id="4e30d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4e30d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4e30d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e30d-111">Permission type</span></span>|<span data-ttu-id="4e30d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4e30d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e30d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e30d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e30d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e30d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4e30d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e30d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e30d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e30d-116">Not supported.</span></span>|
|<span data-ttu-id="4e30d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e30d-117">Application</span></span>|<span data-ttu-id="4e30d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e30d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e30d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e30d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4e30d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e30d-120">Request headers</span></span>
|<span data-ttu-id="4e30d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e30d-121">Header</span></span>|<span data-ttu-id="4e30d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4e30d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e30d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e30d-123">Authorization</span></span>|<span data-ttu-id="4e30d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e30d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e30d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4e30d-125">Accept</span></span>|<span data-ttu-id="4e30d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e30d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e30d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e30d-127">Request body</span></span>
<span data-ttu-id="4e30d-128">No corpo da solicitação, fornece uma representação JSON para o objeto intuneBrandingProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="4e30d-128">In the request body, supply a JSON representation for the intuneBrandingProfileAssignment object.</span></span>

<span data-ttu-id="4e30d-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o intuneBrandingProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="4e30d-129">The following table shows the properties that are required when you create the intuneBrandingProfileAssignment.</span></span>

|<span data-ttu-id="4e30d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e30d-130">Property</span></span>|<span data-ttu-id="4e30d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e30d-131">Type</span></span>|<span data-ttu-id="4e30d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e30d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e30d-133">id</span><span class="sxs-lookup"><span data-stu-id="4e30d-133">id</span></span>|<span data-ttu-id="4e30d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e30d-134">String</span></span>|<span data-ttu-id="4e30d-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="4e30d-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="4e30d-136">destino</span><span class="sxs-lookup"><span data-stu-id="4e30d-136">target</span></span>|[<span data-ttu-id="4e30d-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4e30d-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4e30d-138">Destino de atribuição atribuída à marcação perfil.</span><span class="sxs-lookup"><span data-stu-id="4e30d-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="4e30d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e30d-139">Response</span></span>
<span data-ttu-id="4e30d-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e30d-140">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e30d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e30d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e30d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e30d-142">Request</span></span>
<span data-ttu-id="4e30d-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e30d-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
Content-type: application/json
Content-length: 171

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="4e30d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e30d-144">Response</span></span>
<span data-ttu-id="4e30d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e30d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 220

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





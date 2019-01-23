---
title: Atualizar intuneBrandingProfileAssignment
description: Atualize as propriedades de um objeto intuneBrandingProfileAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7bfdba766221fc27dde6a8b71212620b744c4fc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428995"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="a5e34-103">Atualizar intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="a5e34-103">Update intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="a5e34-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a5e34-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a5e34-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a5e34-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5e34-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a5e34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5e34-107">Atualize as propriedades de um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a5e34-107">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5e34-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a5e34-108">Prerequisites</span></span>
<span data-ttu-id="a5e34-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a5e34-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a5e34-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5e34-111">Permission type</span></span>|<span data-ttu-id="a5e34-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a5e34-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5e34-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5e34-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5e34-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5e34-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a5e34-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5e34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5e34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5e34-116">Not supported.</span></span>|
|<span data-ttu-id="a5e34-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5e34-117">Application</span></span>|<span data-ttu-id="a5e34-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5e34-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5e34-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5e34-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="a5e34-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e34-120">Request headers</span></span>
|<span data-ttu-id="a5e34-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5e34-121">Header</span></span>|<span data-ttu-id="a5e34-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a5e34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5e34-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5e34-123">Authorization</span></span>|<span data-ttu-id="a5e34-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5e34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5e34-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a5e34-125">Accept</span></span>|<span data-ttu-id="a5e34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5e34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5e34-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e34-127">Request body</span></span>
<span data-ttu-id="a5e34-128">No corpo da solicitação, fornece uma representação JSON para o objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a5e34-128">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="a5e34-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a5e34-129">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="a5e34-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5e34-130">Property</span></span>|<span data-ttu-id="a5e34-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5e34-131">Type</span></span>|<span data-ttu-id="a5e34-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5e34-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5e34-133">id</span><span class="sxs-lookup"><span data-stu-id="a5e34-133">id</span></span>|<span data-ttu-id="a5e34-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5e34-134">String</span></span>|<span data-ttu-id="a5e34-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="a5e34-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="a5e34-136">destino</span><span class="sxs-lookup"><span data-stu-id="a5e34-136">target</span></span>|[<span data-ttu-id="a5e34-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a5e34-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a5e34-138">Destino de atribuição atribuída à marcação perfil.</span><span class="sxs-lookup"><span data-stu-id="a5e34-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="a5e34-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5e34-139">Response</span></span>
<span data-ttu-id="a5e34-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5e34-140">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5e34-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5e34-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5e34-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e34-142">Request</span></span>
<span data-ttu-id="a5e34-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5e34-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
Content-type: application/json
Content-length: 171

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="a5e34-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5e34-144">Response</span></span>
<span data-ttu-id="a5e34-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5e34-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





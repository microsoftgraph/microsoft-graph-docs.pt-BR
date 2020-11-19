---
title: Atualizar appleUserInitiatedEnrollmentProfile
description: Atualiza as propriedades de um objeto appleUserInitiatedEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1ec83d3d9f4e8ca06d9f0f92752e9655b9fb469c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49309687"
---
# <a name="update-appleuserinitiatedenrollmentprofile"></a><span data-ttu-id="2d802-103">Atualizar appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="2d802-103">Update appleUserInitiatedEnrollmentProfile</span></span>

<span data-ttu-id="2d802-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d802-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d802-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2d802-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d802-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d802-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d802-107">Atualiza as propriedades de um objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2d802-107">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d802-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d802-108">Prerequisites</span></span>
<span data-ttu-id="2d802-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d802-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d802-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d802-111">Permission type</span></span>|<span data-ttu-id="2d802-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2d802-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d802-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d802-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2d802-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d802-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2d802-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d802-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d802-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d802-116">Not supported.</span></span>|
|<span data-ttu-id="2d802-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d802-117">Application</span></span>|<span data-ttu-id="2d802-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d802-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d802-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d802-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="2d802-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d802-120">Request headers</span></span>
|<span data-ttu-id="2d802-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d802-121">Header</span></span>|<span data-ttu-id="2d802-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2d802-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d802-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d802-123">Authorization</span></span>|<span data-ttu-id="2d802-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d802-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d802-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2d802-125">Accept</span></span>|<span data-ttu-id="2d802-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2d802-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d802-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d802-127">Request body</span></span>
<span data-ttu-id="2d802-128">No corpo da solicitação, forneça uma representação JSON do objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2d802-128">In the request body, supply a JSON representation for the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

<span data-ttu-id="2d802-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="2d802-129">The following table shows the properties that are required when you create the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>

|<span data-ttu-id="2d802-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d802-130">Property</span></span>|<span data-ttu-id="2d802-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d802-131">Type</span></span>|<span data-ttu-id="2d802-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d802-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d802-133">defaultenrollmentidtype</span><span class="sxs-lookup"><span data-stu-id="2d802-133">defaultEnrollmentType</span></span>|[<span data-ttu-id="2d802-134">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="2d802-134">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="2d802-135">O tipo de registro de perfil padrão.</span><span class="sxs-lookup"><span data-stu-id="2d802-135">The default profile enrollment type.</span></span> <span data-ttu-id="2d802-136">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="2d802-136">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="2d802-137">availableEnrollmentTypeOptions</span><span class="sxs-lookup"><span data-stu-id="2d802-137">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="2d802-138">coleção [appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="2d802-138">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="2d802-139">Lista de opções de tipo de registro disponíveis</span><span class="sxs-lookup"><span data-stu-id="2d802-139">List of available enrollment type options</span></span>|
|<span data-ttu-id="2d802-140">id</span><span class="sxs-lookup"><span data-stu-id="2d802-140">id</span></span>|<span data-ttu-id="2d802-141">String</span><span class="sxs-lookup"><span data-stu-id="2d802-141">String</span></span>|<span data-ttu-id="2d802-142">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="2d802-142">The GUID for the object</span></span>|
|<span data-ttu-id="2d802-143">displayName</span><span class="sxs-lookup"><span data-stu-id="2d802-143">displayName</span></span>|<span data-ttu-id="2d802-144">String</span><span class="sxs-lookup"><span data-stu-id="2d802-144">String</span></span>|<span data-ttu-id="2d802-145">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="2d802-145">Name of the profile</span></span>|
|<span data-ttu-id="2d802-146">description</span><span class="sxs-lookup"><span data-stu-id="2d802-146">description</span></span>|<span data-ttu-id="2d802-147">String</span><span class="sxs-lookup"><span data-stu-id="2d802-147">String</span></span>|<span data-ttu-id="2d802-148">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="2d802-148">Description of the profile</span></span>|
|<span data-ttu-id="2d802-149">prioridade</span><span class="sxs-lookup"><span data-stu-id="2d802-149">priority</span></span>|<span data-ttu-id="2d802-150">Int32</span><span class="sxs-lookup"><span data-stu-id="2d802-150">Int32</span></span>|<span data-ttu-id="2d802-151">Prioridade, 0 é a maior</span><span class="sxs-lookup"><span data-stu-id="2d802-151">Priority, 0 is highest</span></span>|
|<span data-ttu-id="2d802-152">plataforma</span><span class="sxs-lookup"><span data-stu-id="2d802-152">platform</span></span>|[<span data-ttu-id="2d802-153">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="2d802-153">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="2d802-154">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2d802-154">The platform of the Device.</span></span> <span data-ttu-id="2d802-155">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="2d802-155">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="2d802-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d802-156">createdDateTime</span></span>|<span data-ttu-id="2d802-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d802-157">DateTimeOffset</span></span>|<span data-ttu-id="2d802-158">Hora de criação do perfil</span><span class="sxs-lookup"><span data-stu-id="2d802-158">Profile creation time</span></span>|
|<span data-ttu-id="2d802-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d802-159">lastModifiedDateTime</span></span>|<span data-ttu-id="2d802-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d802-160">DateTimeOffset</span></span>|<span data-ttu-id="2d802-161">Hora da última modificação do perfil</span><span class="sxs-lookup"><span data-stu-id="2d802-161">Profile last modified time</span></span>|



## <a name="response"></a><span data-ttu-id="2d802-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d802-162">Response</span></span>
<span data-ttu-id="2d802-163">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d802-163">If successful, this method returns a `200 OK` response code and an updated [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d802-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d802-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d802-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d802-165">Request</span></span>
<span data-ttu-id="2d802-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d802-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
Content-type: application/json
Content-length: 439

{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "device",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "company",
      "enrollmentType": "device"
    }
  ],
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "platform": "androidForWork"
}
```

### <a name="response"></a><span data-ttu-id="2d802-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d802-167">Response</span></span>
<span data-ttu-id="2d802-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d802-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "device",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "company",
      "enrollmentType": "device"
    }
  ],
  "id": "5a11d98e-d98e-5a11-8ed9-115a8ed9115a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "platform": "androidForWork",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





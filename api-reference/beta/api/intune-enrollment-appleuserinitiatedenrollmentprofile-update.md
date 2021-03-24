---
title: Atualizar appleUserInitiatedEnrollmentProfile
description: Atualize as propriedades de um objeto appleUserInitiatedEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca6dda640ceaadb4420a41cf4bfd0e147f3d29f2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146059"
---
# <a name="update-appleuserinitiatedenrollmentprofile"></a><span data-ttu-id="8ceec-103">Atualizar appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="8ceec-103">Update appleUserInitiatedEnrollmentProfile</span></span>

<span data-ttu-id="8ceec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ceec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ceec-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8ceec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ceec-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ceec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ceec-107">Atualize as propriedades de [um objeto appleUserInitiatedEnrollmentProfile.](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8ceec-107">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ceec-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8ceec-108">Prerequisites</span></span>
<span data-ttu-id="8ceec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ceec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ceec-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ceec-111">Permission type</span></span>|<span data-ttu-id="8ceec-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ceec-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ceec-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ceec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ceec-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ceec-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8ceec-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ceec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ceec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ceec-116">Not supported.</span></span>|
|<span data-ttu-id="8ceec-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ceec-117">Application</span></span>|<span data-ttu-id="8ceec-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ceec-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ceec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ceec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="8ceec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ceec-120">Request headers</span></span>
|<span data-ttu-id="8ceec-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ceec-121">Header</span></span>|<span data-ttu-id="8ceec-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8ceec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ceec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ceec-123">Authorization</span></span>|<span data-ttu-id="8ceec-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ceec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ceec-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8ceec-125">Accept</span></span>|<span data-ttu-id="8ceec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ceec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ceec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ceec-127">Request body</span></span>
<span data-ttu-id="8ceec-128">No corpo da solicitação, fornece uma representação JSON para o [objeto appleUserInitiatedEnrollmentProfile.](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8ceec-128">In the request body, supply a JSON representation for the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

<span data-ttu-id="8ceec-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="8ceec-129">The following table shows the properties that are required when you create the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>

|<span data-ttu-id="8ceec-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ceec-130">Property</span></span>|<span data-ttu-id="8ceec-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ceec-131">Type</span></span>|<span data-ttu-id="8ceec-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ceec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ceec-133">defaultEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="8ceec-133">defaultEnrollmentType</span></span>|[<span data-ttu-id="8ceec-134">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="8ceec-134">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="8ceec-135">O tipo de registro de perfil padrão.</span><span class="sxs-lookup"><span data-stu-id="8ceec-135">The default profile enrollment type.</span></span> <span data-ttu-id="8ceec-136">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="8ceec-136">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="8ceec-137">availableEnrollmentTypeOptions</span><span class="sxs-lookup"><span data-stu-id="8ceec-137">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="8ceec-138">[Coleção appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="8ceec-138">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="8ceec-139">Lista de opções de tipo de registro disponível</span><span class="sxs-lookup"><span data-stu-id="8ceec-139">List of available enrollment type options</span></span>|
|<span data-ttu-id="8ceec-140">id</span><span class="sxs-lookup"><span data-stu-id="8ceec-140">id</span></span>|<span data-ttu-id="8ceec-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ceec-141">String</span></span>|<span data-ttu-id="8ceec-142">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="8ceec-142">The GUID for the object</span></span>|
|<span data-ttu-id="8ceec-143">displayName</span><span class="sxs-lookup"><span data-stu-id="8ceec-143">displayName</span></span>|<span data-ttu-id="8ceec-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ceec-144">String</span></span>|<span data-ttu-id="8ceec-145">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="8ceec-145">Name of the profile</span></span>|
|<span data-ttu-id="8ceec-146">descrição</span><span class="sxs-lookup"><span data-stu-id="8ceec-146">description</span></span>|<span data-ttu-id="8ceec-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ceec-147">String</span></span>|<span data-ttu-id="8ceec-148">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="8ceec-148">Description of the profile</span></span>|
|<span data-ttu-id="8ceec-149">prioridade</span><span class="sxs-lookup"><span data-stu-id="8ceec-149">priority</span></span>|<span data-ttu-id="8ceec-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8ceec-150">Int32</span></span>|<span data-ttu-id="8ceec-151">Prioridade, 0 é mais alta</span><span class="sxs-lookup"><span data-stu-id="8ceec-151">Priority, 0 is highest</span></span>|
|<span data-ttu-id="8ceec-152">plataforma</span><span class="sxs-lookup"><span data-stu-id="8ceec-152">platform</span></span>|[<span data-ttu-id="8ceec-153">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="8ceec-153">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="8ceec-154">A plataforma do Dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8ceec-154">The platform of the Device.</span></span> <span data-ttu-id="8ceec-155">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="8ceec-155">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="8ceec-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ceec-156">createdDateTime</span></span>|<span data-ttu-id="8ceec-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ceec-157">DateTimeOffset</span></span>|<span data-ttu-id="8ceec-158">Tempo de criação de perfil</span><span class="sxs-lookup"><span data-stu-id="8ceec-158">Profile creation time</span></span>|
|<span data-ttu-id="8ceec-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ceec-159">lastModifiedDateTime</span></span>|<span data-ttu-id="8ceec-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ceec-160">DateTimeOffset</span></span>|<span data-ttu-id="8ceec-161">Tempo de última modificação do perfil</span><span class="sxs-lookup"><span data-stu-id="8ceec-161">Profile last modified time</span></span>|



## <a name="response"></a><span data-ttu-id="8ceec-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ceec-162">Response</span></span>
<span data-ttu-id="8ceec-163">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ceec-163">If successful, this method returns a `200 OK` response code and an updated [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ceec-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ceec-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ceec-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ceec-165">Request</span></span>
<span data-ttu-id="8ceec-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ceec-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8ceec-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ceec-167">Response</span></span>
<span data-ttu-id="8ceec-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ceec-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





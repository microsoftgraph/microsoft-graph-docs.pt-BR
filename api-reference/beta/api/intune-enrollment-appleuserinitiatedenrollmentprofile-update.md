---
title: Atualizar appleUserInitiatedEnrollmentProfile
description: Atualiza as propriedades de um objeto appleUserInitiatedEnrollmentProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6518f3cd17c781c9ecb1ba41865ae31ce14af1a6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813457"
---
# <a name="update-appleuserinitiatedenrollmentprofile"></a><span data-ttu-id="4084a-103">Atualizar appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="4084a-103">Update appleUserInitiatedEnrollmentProfile</span></span>

> <span data-ttu-id="4084a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4084a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4084a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4084a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4084a-106">Atualiza as propriedades de um objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4084a-106">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4084a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4084a-107">Prerequisites</span></span>
<span data-ttu-id="4084a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4084a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4084a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4084a-110">Permission type</span></span>|<span data-ttu-id="4084a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4084a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4084a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4084a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4084a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4084a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4084a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4084a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4084a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4084a-115">Not supported.</span></span>|
|<span data-ttu-id="4084a-116">Application</span><span class="sxs-lookup"><span data-stu-id="4084a-116">Application</span></span>|<span data-ttu-id="4084a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4084a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4084a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4084a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="4084a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4084a-119">Request headers</span></span>
|<span data-ttu-id="4084a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4084a-120">Header</span></span>|<span data-ttu-id="4084a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4084a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4084a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4084a-122">Authorization</span></span>|<span data-ttu-id="4084a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4084a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4084a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4084a-124">Accept</span></span>|<span data-ttu-id="4084a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4084a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4084a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4084a-126">Request body</span></span>
<span data-ttu-id="4084a-127">No corpo da solicitação, forneça uma representação JSON do objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4084a-127">In the request body, supply a JSON representation for the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

<span data-ttu-id="4084a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="4084a-128">The following table shows the properties that are required when you create the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>

|<span data-ttu-id="4084a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4084a-129">Property</span></span>|<span data-ttu-id="4084a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4084a-130">Type</span></span>|<span data-ttu-id="4084a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4084a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4084a-132">defaultenrollmentidtype</span><span class="sxs-lookup"><span data-stu-id="4084a-132">defaultEnrollmentType</span></span>|[<span data-ttu-id="4084a-133">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="4084a-133">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="4084a-134">O tipo de registro de perfil padrão.</span><span class="sxs-lookup"><span data-stu-id="4084a-134">The default profile enrollment type.</span></span> <span data-ttu-id="4084a-135">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="4084a-135">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="4084a-136">availableEnrollmentTypeOptions</span><span class="sxs-lookup"><span data-stu-id="4084a-136">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="4084a-137">coleção [appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="4084a-137">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="4084a-138">Lista de opções de tipo de registro disponíveis</span><span class="sxs-lookup"><span data-stu-id="4084a-138">List of available enrollment type options</span></span>|
|<span data-ttu-id="4084a-139">id</span><span class="sxs-lookup"><span data-stu-id="4084a-139">id</span></span>|<span data-ttu-id="4084a-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4084a-140">String</span></span>|<span data-ttu-id="4084a-141">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="4084a-141">The GUID for the object</span></span>|
|<span data-ttu-id="4084a-142">displayName</span><span class="sxs-lookup"><span data-stu-id="4084a-142">displayName</span></span>|<span data-ttu-id="4084a-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4084a-143">String</span></span>|<span data-ttu-id="4084a-144">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="4084a-144">Name of the profile</span></span>|
|<span data-ttu-id="4084a-145">description</span><span class="sxs-lookup"><span data-stu-id="4084a-145">description</span></span>|<span data-ttu-id="4084a-146">String</span><span class="sxs-lookup"><span data-stu-id="4084a-146">String</span></span>|<span data-ttu-id="4084a-147">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="4084a-147">Description of the profile</span></span>|
|<span data-ttu-id="4084a-148">prioridade</span><span class="sxs-lookup"><span data-stu-id="4084a-148">priority</span></span>|<span data-ttu-id="4084a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="4084a-149">Int32</span></span>|<span data-ttu-id="4084a-150">Prioridade, 0 é a maior</span><span class="sxs-lookup"><span data-stu-id="4084a-150">Priority, 0 is highest</span></span>|
|<span data-ttu-id="4084a-151">platform</span><span class="sxs-lookup"><span data-stu-id="4084a-151">platform</span></span>|[<span data-ttu-id="4084a-152">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="4084a-152">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="4084a-153">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4084a-153">The platform of the Device.</span></span> <span data-ttu-id="4084a-154">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4084a-154">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="4084a-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4084a-155">createdDateTime</span></span>|<span data-ttu-id="4084a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4084a-156">DateTimeOffset</span></span>|<span data-ttu-id="4084a-157">Hora de criação do perfil</span><span class="sxs-lookup"><span data-stu-id="4084a-157">Profile creation time</span></span>|
|<span data-ttu-id="4084a-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4084a-158">lastModifiedDateTime</span></span>|<span data-ttu-id="4084a-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4084a-159">DateTimeOffset</span></span>|<span data-ttu-id="4084a-160">Hora da última modificação do perfil</span><span class="sxs-lookup"><span data-stu-id="4084a-160">Profile last modified time</span></span>|



## <a name="response"></a><span data-ttu-id="4084a-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="4084a-161">Response</span></span>
<span data-ttu-id="4084a-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4084a-162">If successful, this method returns a `200 OK` response code and an updated [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4084a-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4084a-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="4084a-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4084a-164">Request</span></span>
<span data-ttu-id="4084a-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4084a-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4084a-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="4084a-166">Response</span></span>
<span data-ttu-id="4084a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4084a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




